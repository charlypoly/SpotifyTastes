# SpotifyTastes


### Types

```typescript
interface UserProfile {
  id: string
  pseudo: string
  tracks: SpotifyCollector.WeightedTracks | Set<SpotifyCollector.UserTracks>
}
type pseudo = string;
```

See [SpotifyCollector types](https://github.com/thefrenchhouse/SpotifyCollector)

### Services

```typescript
commonGenres(UserProfile[], limit=5): {[genre:string]: pseudo[]}
commonArtists(UserProfile[], limit=5): {[artistName:string]: pseudo[]}
bestGenres(UserProfile[], limit=5): string[]
bestArtists(UserProfile[], limit=5): string[]
```
