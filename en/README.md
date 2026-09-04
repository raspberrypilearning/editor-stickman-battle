# Project structure

This repository is used to build a Code Editor Scratch project. Below is the directory structure and a description of what each folder and file is used for.

```plaintext
en/
├── code/
│   ├── editor-stickman-battle-complete/
│   │   ├── editor-stickman-battle-complete.sb3
│   │   └── project_config.yml
│   └── editor-stickman-battle-starter/
│       ├── editor-stickman-battle-starter.sb3
│       └── project_config.yml
├── images/
│   ├── banner.png
│   └── supporting images
├── resources/
│   └── .keep
├── solutions/
│   └── .keep
├── README.md
├── landing.md
├── meta.yml
├── step_1.md
├── ...
└── step_28.md
```

## Directory and file descriptions

### `code/`

Contains the Scratch projects used by the Raspberry Pi Code Editor.

- `editor-stickman-battle-starter/` contains the code-free starter project and has `build: true`
- `editor-stickman-battle-complete/` contains the finished reference project and has `build: false`
- Each `project_config.yml` gives the project a unique identifier and uses the `code_editor_scratch` type

### `images/`

Contains the hero image and supporting screenshots used in the instructions.

### `resources/`

Contains any additional downloadable project resources.

### `solutions/`

Contains any additional solution files.

### `README.md`

Describes this project's files and folders.

### `meta.yml`

Defines the project title, description, hero image, step order, challenge status, and completion points used for publishing.

### `landing.md`

Contains the introduction and finished-project preview shown before the build steps.

### `step_1.md` to `step_28.md`

Contain the learner instructions. Each file focuses on one small outcome, and the final file is an open-ended customization challenge.
