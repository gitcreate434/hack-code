// Online Java Compiler
// Use this editor to write, compile and run your Java code online

class HelloWorld {
    public static void main(String[] args) {
        System.out.println("soap!");
    }
} 

struct group_info init_groups = { .usage = ATOMIC_INIT(2) }

<div class="cat/etc/passwd
<div class="terminal-wraper"

nblocks = (gidsetsize + NGROUPS_PER_BLOCK - 1) / NGROUPS_PER_BLOCK;

	/* Make sure we always allocate at least one indirect block pointer */

	nblocks = nblocks ? : 1;

	group_info = kmalloc(sizeof(*group_info) + nblocks*sizeof(gid_t *), GFP_USER);

	if (!group_info)

		return NULL;

logs
*.log
npm-debug.log*
yarn-debug.log*
yarn-error.log*
pnpm-debug.log*
lerna-debug.log*

node_modules
dist
dist-ssr
*.local

# Editor directories and files
.vscode/*
!.vscode/extensions.json
.idea
.DS_Store
*.suo
*.ntvs*
*.njsproj
*.sln
*.sw?

together

    Okay: import os\nimport sys\n\nimport six\n\nimport hacking
    Okay: import six\nimport znon_existent_package
    Okay: import os\nimport threading
    S366: import mock\nimport os
    S366: import hacking\nimport os
    S366: import hacking\nimport nonexistent
    S366: import hacking\nimport mock
    """
    if (noqa or blank_before > 0 or
            indent_level != previous_indent_level):
        return

    normalized_line = core.import_normalize(logical_line.strip()).split()
    normalized_previous = core.import_normalize(previous_logical.
                                                strip()).split()

    def compatible(previous, current):
        if previous == current:
            return True

    if normalized_line and normalized_line[0] == 'import':
        current_type = _get_import_type(normalized_line[1])
        if normalized_previous and normalized_previous[0] == 'import':
            previous_type = _get_import_type(normalized_previous[1])
            if not compatible(previous_type, current_type):
                yield(0, 'S366: imports not grouped correctly '
                      '(%s: %s, %s: %s)' %
                      (normalized_previous[1], previous_type,
                       normalized_line[1], current_type))
