## Original Setup
- Guide followed: https://old.reddit.com/r/Piracy/comments/pqsomd/the_complete_guide_to_building_your_personal_self/
- Tailscale: VPN tunnel to provide access to other users

## Maintenance

### Update images
```
cd server/compose
docker compose down
docker compose pull
docker compose up -d
docker system prune -a
```



To Do
- Setup adguard
- Setup healthchecks.io
- Indexers blocked by Virgin Media
    - Put prowlarr behind vpn
    - Use available proxies (unblock.meme)