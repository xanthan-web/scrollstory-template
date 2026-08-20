---
title: Template Instructions
layout: base
---

# Using This ScrollStory Template

This page guides you through customizing this template for your own ScrollStory essay. Once you're done editing (or feel like you got the hang of it), **you can delete this file**—it's just for getting started.


## What You Have
This template includes:
- **The essay itself, as your homepage** (`index.md`). A visitor lands in the
  scrollstory rather than on a page describing one. It ships as a demo called
  "The Forest" that uses every ScrollStory component at least once.
- **Its images** in `images/` at the top level, next to `index.md`
- **About page** for general information about you or your project (`about.md`)
- **Bibliography page** for your sources (`bibliography.md`)


## Using AI to Build Your ScrollStory

ScrollStories have more moving parts than a standard page—background images, scrollyboxes, carousels, pacing parameters. AI assistants handle this well because Xanthan's components use named parameters and clear structure.

**A good opening prompt:**

> "I'm building a ScrollStory essay using the Xanthan Jekyll framework. Here's my essay file: [paste your `index.md`]. I want to add a scrollybox with a background image that shows text overlaid on a full-screen forest photo. The image is at `images/forest.jpg`. Can you show me the include tag to use?"

Or to get started from scratch:

> "I'm using the Xanthan ScrollStory template. I want to create an essay about the history of urban parks. Can you help me outline the essay structure and suggest which ScrollStory components would work best for each section?"

AI is especially useful for:
- Writing or editing the scrollybox `box-content` text
- Adjusting `above-box-space` and `below-box-space` for pacing
- Troubleshooting broken Liquid tags
- Explaining what any component parameter does

The [ScrollStory documentation](docs/scrollstories/) shows every component with its full parameter list—paste relevant sections into your AI conversation as needed.


## Start Editing!

If you're not familiar with [editing your site on GitHub](docs/getting-started/editing-in-github.md), read through the directions on how to do that. 



### 1. Make the Essay Yours (`index.md`)

`index.md` **is** your essay — it is what a visitor sees first. Start at the
top:
- Change `title`, `header-title` and `header-subtitle` in the front matter
- Replace `header-image` with your own opening picture
- Then work down through the scrollyboxes, replacing text as you go


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

Open `index.md` to see your essay content. The file includes:

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

1. **Edit the text** in `index.md`
   - Keep the special tags (like `{% include scrollybox/bg.html %}`)
   - Replace the text inside scrollboxes with your content
   - Update image paths to point to your own images

2. **Add your images** to `images/`:
   - Upload ALL images here
   - Use descriptive filenames (e.g., `forest-view.jpg`, `historical-map.png`)


3. **Learn the components** from the [ScrollStory documentation](/docs/scrollstories/):
   - How to add background images
   - How to switch between images
   - How to create side-scrolling sections


## Adding Images

### Where to Put Images

Put all your essay images in the `images/` folder beside `index.md`:
```
index.md
images/
├── background-1.jpg
├── background-2.jpg
└── detail-photo.png
```
That is why the essay refers to them as `images/background-1.jpg` — the path is
relative to the page.


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
3. **Remove the docs link from the top nav** Remove the title and url lines (in `_data/top-nav.yml`)
 
---

**Questions?** Check the [Xanthan documentation](https://xanthan-web.github.io/xanthan/) or [report an issue](https://github.com/xanthan-web/scrollstory-template/issues).
