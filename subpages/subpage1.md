# A subpage

- [a relative link to another subpage](subpage2.md) - `(subpage2.md)`
    - This one results in `/#/subpage2`, which gets a 404
- [another relative link to the same subpage](./subpage2.md) - `(./subpage2.md)`
    - This one results in `/#/./subpage2`, which also gests a 404
- [a relative link to readme](../README.md)
    - This one results in `/#/../README`
    - It works if you are serving at `/`, but it fails if you are serving at a sub folder (i.e. github pages of a repository)