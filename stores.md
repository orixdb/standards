OrixDB standards | Strores
==========================

An OrixDB store is a folder containing:

- A manifest file named "rixifest.json", that contains the store's metadata
- A folder named "tmp", that serve as draft
- A folder name "logs", that contains the log files
- A folder named "scattereds", that contains a file for each orphan object
- A folder named "collections", that contains a subfolder for each collection


## Store metadata

- name: String
- slug: String
- type: "live" | "backup" | "archive"
- ordered: Bool
- defaults: Object
    - buffering: bool
    - logging: "off" | "minimal" | "normal" | "detailed"
    - api-port: Number (7979)
    - cluster-port: Number (79000...)