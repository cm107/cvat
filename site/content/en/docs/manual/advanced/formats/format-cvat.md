---
linkTitle: 'CVAT'
weight: 1
---

This is CVAT's native annotation format,
which fully supports all of CVAT's annotation features.
It is ideal for creating data backups.

For more information, see:

- [Format specification](/docs/manual/advanced/xml_format/)
- [Dataset examples](https://github.com/cvat-ai/datumaro/tree/v0.3/tests/assets/cvat_dataset)

## CVAT for image export

For export of images:

- Supported annotations: Bounding Boxes, Polygons, Polylines,
  Points, Cuboids, Skeletons, Tags, Tracks
- Attributes: Supported.
- Tracks: Supported (tracks are split by frames).

The downloaded file is a zip archive with following structure:

```bash
taskname.zip/
├── images/
|   ├── img1.png
|   └── img2.jpg
└── annotations.xml
```

## CVAT for video export

For export of images:

- Supported annotations: Bounding Boxes, Polygons, Polylines,
  Points, Cuboids, Skeletons, Tags, Tracks
- Attributes: Supported.
- Tracks: Supported (tracks are split by frames).
- Shapes are exported as single-frame tracks

Downloaded file is a zip archive with following structure:

```bash
taskname.zip/
├── images/
|   ├── frame_000000.png
|   └── frame_000001.png
└── annotations.xml
```

## CVAT loader

Uploaded file: either an XML file or a
.zip file containing the aforementioned structures.
