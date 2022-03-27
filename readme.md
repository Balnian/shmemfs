# SHMEMFS
A library for easy distributed and parallel access to Filesystem resources. This project is inspired by the BCL library.

## Roadmap
### File access

#### Read features:

- [ ] One reader that distribute to all the others PE
- [ ] Multiple readers on a shared file 
- [ ] Built-in split heuristics based on [by line, on char delimiter
- [ ] Allow user provided split heuristics


#### Write features
- [ ] One writer collecting all the other PE data
- [ ] Multiple writers on a shared file (TBD)

```cpp
template <typename T>
    file f = file_map(int root_PE, string Path, T split_heuristic );
```

