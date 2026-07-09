# Visual Viewer Reference

The repository includes a static viewer at:

```text
viewer/graph-viewer.html
```

It can be opened directly in a browser. It does not require a server.

## What the viewer is for

Use the viewer when a user wants a fast visual layer on top of the Markdown graph:

- left rail: deposits and surprising connections
- center: draggable and zoomable graph canvas
- right panel: node meaning, connected nodes, and next actions
- import: load a custom JSON graph file

## Viewer data shape

The viewer accepts this JSON shape:

```json
{
  "title": "My Content Graph",
  "groups": {
    "core": { "label": "Core", "color": "#185c47" }
  },
  "nodes": [
    {
      "id": "brain",
      "label": "Content Brain",
      "group": "core",
      "x": 600,
      "y": 360,
      "size": 86,
      "kind": "central",
      "desc": "What this node means.",
      "actions": ["Next action one", "Next action two"]
    }
  ],
  "edges": [
    {
      "source": "brain",
      "target": "next-node",
      "label": "why they connect",
      "type": "primary"
    }
  ],
  "deposits": ["brain"]
}
```

## Edge types

- `primary`: strong visible relationship
- `support`: child or supporting relationship
- `surprise`: non-obvious useful connection, highlighted in gold

## Node layout

The viewer uses fixed `x` and `y` coordinates. When generating data:

- keep the central node near `x: 600`, `y: 360`
- keep major groups around the center
- use `size` for cluster nodes
- use `w` for pill-shaped leaf nodes
- keep labels short enough to fit

## Privacy checklist

Before sharing a generated viewer JSON publicly, remove:

- private file paths
- thread IDs
- unpublished client, business, or personal details
- raw diary or relationship material
- internal delegation notes
- claims about guaranteed growth, traffic, or viral outcomes

Public examples should show the reusable workflow, not the user's private archive.
