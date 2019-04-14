# Open Flash DB Registry

Registry of SWF files available on the internet.

```typescript
interface Movie {
  /**
   * Unique name identifying the movie.
   */
  name: string;

  /**
   * Primary URI of the SWF file.
   */
  uri: string;

  /**
   * Array of mirror URIs.
   */
  mirrors: string[];

  /**
   * Free-form description of the movie.
   */
  description?: string;

  /**
   * Author of the SWF file. Format: `name <email> (uri)` (`email` and `uri` are optional).
   */
  author?: string;

  /**
   * Main URI where the SWF file is embedded / accessible.
   */
  homepage?: string;

  /**
   * Size of the file in bytes.
   */
  size: number;

  /**
   * Hashes of the file.
   */
  hashes: {
    /**
     * SHA256 hash encoded as a hex string.
     */
    sha256?: string;
  };
}
```
