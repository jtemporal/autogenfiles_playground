# AutoGenFiles Playground

AutoGenFiles collection of examples.

## How to use this repo

Install autogenfiles, go into the example you want to see then run the command outlined in said example REAME.md
 
### Examples

#### Operation Simplicity

The simplest use case possible: `templates/` has only files to be rendered, variables file follow the default naming, and output go in the root of project.

```console
operation_simplicity
├── OperationSimplicity.md  -> automatically generated from templates folder
├── README.md               -> general instructions
├── templates               -> templates folder
│   └── {{ project_name }}.md
└── variables.yaml          -> variables file
```

#### Operation Subfolders

This time `templates/` has a subfolder structure that needs to be followed, the output go in the root but follow the subfolder structure from `templates/`, and variable files has a non-default naming.

```console
operation_subfolders
├── REAME.md          -> general instructions
├── _posts            -> atomatically generated from templates folder
├── projects          -> automatically generated from templates folder
├── templates         -> templates folder
│   ├── _posts
│   └── projects
└── variables.ini     -> variables file
```

#### Operation Rendered

The most complex case so far: `templates/` has a subfolder structure that needs to be followed, the output goes into an output directory called `rendered/` that follows the subfolder structure from `templates/`, and variable file has a non-default naming.

```console
operation_rendered
├── REAME.md       -> general instructions
├── rendered       -> automatically generated from templates folder
│   ├── _posts
│   └── projects
├── templates      -> templates folder
│   ├── _posts
│   └── projects
└── variables.ini  -> variables file
```
