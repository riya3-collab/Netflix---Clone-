# Netflix-Clone-90LPA 🎬

### Live: https://riya3-collab.github.io/Netflix-Clone-90LPA/

## System Design Concepts Used
1. **CDN Edge Caching:** LRU Cache simulates CloudFlare/Akamai edge nodes
2. **LRU Eviction:** Least Recently Used algorithm for cache management  
3. **Low Latency:** Cache hits <50ms, Misses 500ms+ from origin
4. **Horizontal Scale:** Stateless frontend, can add 1000+ edge nodes

## Tech Stack
- **Frontend:** HTML5, CSS3, Vanilla JS
- **Hosting:** GitHub Pages - Free, Global CDN, HTTPS
- **Caching:** In-memory LRU Cache - O(1) get/put

## Interview Talking Points
Q: How does Netflix reduce latency?  
A: CDN Edge Caching with LRU eviction. Hot content stays at edge near user. My demo shows 90%+ hit rate after warmup.

Q: What if cache full?  
A: LRU evicts least recently used movie. Capacity=3 for demo, production=TBs.

**Built for Microsoft L60 SDE 