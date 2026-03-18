# Complete Open Source Docs Platform

This stack gives you a full documentation CMS with hosting:
- **Wiki.js**: rich docs editor, page management, auth, permissions
- **PostgreSQL**: persistent database
- **Caddy**: HTTPS reverse proxy (optional in local, enabled in production profile)

No GitHub OAuth is required.

## 1. Prepare environment

```bash
cd ops/docs-platform
cp .env.example .env
```

Edit `.env` with secure values.

## 2. Run locally (CMS + DB)

```bash
docker-compose --env-file .env up -d db wikijs
```

Open:
- `http://localhost:3000`

On first launch, Wiki.js setup wizard appears:
1. Create admin account (email/password)
2. Confirm database connection (already wired)
3. Finish installation

## 3. Run in production on VPS (with HTTPS)

DNS requirement:
- Point `docs.yourdomain.com` to your VPS public IP

In `.env`, set:
- `DOCS_DOMAIN=docs.yourdomain.com`
- `WIKI_SSL_ACTIVE=true`

Start full stack:

```bash
docker-compose --env-file .env --profile prod up -d
```

Open:
- `https://docs.yourdomain.com`

## 4. Day-to-day admin workflow

Inside Wiki.js:
1. Create/edit pages in admin/editor UI
2. Organize docs with paths like `/guide/getting-started`
3. Publish/unpublish instantly
4. Manage users and permissions in Administration panel

## 5. Backups (important)

Database backup:

```bash
docker-compose --env-file .env exec -T db pg_dump -U "$POSTGRES_USER" "$POSTGRES_DB" > wikidb-backup.sql
```

Restore:

```bash
cat wikidb-backup.sql | docker-compose --env-file .env exec -T db psql -U "$POSTGRES_USER" "$POSTGRES_DB"
```

## 6. Updates

```bash
docker-compose --env-file .env pull
docker-compose --env-file .env up -d
```

## Notes

- This stack is independent from the old static `/admin` flow.
- You can keep Hugo for public marketing pages if you want, and run docs on subdomain via Wiki.js.
- If you want SSO later (GitHub/Google), Wiki.js supports it in Authentication settings.
