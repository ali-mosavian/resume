# Resume

My CV, published at https://ali-mosavian.github.io/resume/.

`resume.yaml` and `headshot.jpg` are the content; [resume-builder](https://github.com/ali-mosavian/resume-builder), a submodule in `builder/`, turns them into the page, PDFs and Word documents. A push to `main` publishes.

```bash
git clone --recurse-submodules https://github.com/ali-mosavian/resume.git
```

```bash
uv run --project builder resume build --cv resume.yaml --theme split --template builder/templates/split.docx --out build
```

Update the builder with `git submodule update --remote builder` and commit.
