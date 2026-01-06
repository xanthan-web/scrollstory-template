---
title: Template Instructions
layout: base
---

# Using This ScrollStory Template

**Welcome!** This page guides you through customizing this template for your own ScrollStory essay. Once you're done or just like tidying up, **can you delete this file**—it's just for getting started.


## What You Have
This template includes:
- **Homepage** that introduces your essay (index.md)
- **Sample ScrollStory essay** in the `/your-story/` folder. You'll rename this for your project.
- **About page** for general information about you or your project (about.md)
- **Bibliography page** for your sources (bibliography.md)


## Start Editing!

If you're not familiar with [editing your site on GitHub](docs/getting-started/editing-in-github.md), read through the directions on how to do that. 



### 1. Customize the Homepage (`index.md`)

Edit `index.md` in the root folder to:
- Change the title and introduction
- Introduce your project, etc.


### 2. Edit the About Page (`about.md`)
Replace the sample content with:
- Information about you (author bio)
- Context for your essay or project
- Any acknowledgments or credits


### 3. Update the Bibliography (`bibliography.md`)
Add your sources and references:
- Books, articles, websites
- Images sources and credits
- Data sources


## Editing Your ScrollStory

### Understanding the Essay Structure

Open `/your-story/index.md` to see your essay content. The file includes:

**Front Matter (top of file):**
```yaml
---
layout: scrollstory
title: Your Essay Title
---
```

**ScrollStory Components:**
- Background images that appear as you scroll
- Text "scrollboxes" that overlay the images
- Different scrolling effects (sticky, switching, side-scrolling)

### Replacing Sample Content

1. **Edit the text** in `scrollstory/index.md`:
   - Keep the special tags (like `{% include scrollybox/bg.html %}`)
   - Replace the text inside scrollboxes with your content
   - Update image paths to point to your own images

2. **Add your images** to `scrollstory/images/`:
   - Upload your background images here
   - Use descriptive filenames (e.g., `forest-view.jpg`, `historical-map.png`)
   - Update image paths in your essay

3. **Learn the components** from the [ScrollStory documentation](/docs/scrollstories/):
   - How to add background images
   - How to switch between images
   - How to create side-scrolling sections

## Renaming Your Essay Folder

Want to rename `/scrollstory/` to match your essay topic? Here's how:

1. **Rename the folder** to your essay title:
   - Example: `/scrollstory/` → `/forest-history/`
   - Keep the name lowercase with hyphens (no spaces)

2. **Update navigation** in `_data/top-nav.yml`:
   - Find the line with `/scrollstory`
   - Change it to `/forest-history` (or your folder name)

3. **Update homepage link** in `index.md`:
   - Find links pointing to `/scrollstory`
   - Update them to your new folder name

## Adding Images

### Where to Put Images

Put all your essay images in your essay folder's `images/` directory:
```
your-story/
├── index.md
└── images/
    ├── background-1.jpg
    ├── background-2.jpg
    └── detail-photo.png
```


## Getting Help

### Xanthan Documentation
- **Browse local docs**: `/docs/` folder in your repository
- **ScrollStory guides**: `/docs/scrollstories/` for detailed scrolling techniques
- **Online docs**: [xanthan-web.github.io/xanthan/docs/](https://xanthan-web.github.io/xanthan/docs/)

### AI Assistance
Use AI tools like Claude or ChatGPT for help:
- "How do I change the background image in my ScrollStory?"
- "Can you help me add a new scrolling section?"
- "How do I fix this error in my code?"

See the [Using AI Assistance](https://xanthan-web.github.io/xanthan/docs/content-design/using-ai-assistance) guide for tips.



## Clean Up When Done

Once you're comfortable working with your site:
1. **If you want, delete this file** (`instructions.md`)
2. **Remove it from the top nav** Remove the title and url lines (in `_data/top-nav.yml`)

---

{: .text-center .text-muted}
**Questions?** Check the [Xanthan documentation](https://xanthan-web.github.io/xanthan/) or [report an issue](https://github.com/xanthan-web/scrollstory-template/issues).
