# Cri Smile Games Blog Content

This repository contains all the blog posts for the Cri Smile Games website. The blog automatically pulls content from this repository, so any changes you make here will appear on the live site.

## 📁 Repository Structure

```
cri-smile-blog-content/
├── posts/
│   ├── index.json          # Post metadata (IMPORTANT!)
│   ├── welcome-post.md     # Blog post files
│   ├── dev-update-1.md     # Blog post files
│   └── ...                 # More blog posts
├── images/                 # Optional: Blog images
└── README.md              # This file
```

## ✍️ How to Add a New Blog Post

### Step 1: Create the Markdown File

1. Go to the `posts/` folder
2. Click **"Add file"** → **"Create new file"**
3. Name your file using this format: `your-post-title.md`
   - Use lowercase letters
   - Replace spaces with hyphens (-)
   - Example: `development-update-2.md`

### Step 2: Write Your Post

Use this template for your post:

```markdown
# Your Amazing Post Title

Your introduction paragraph goes here. Make it engaging!

## Section 1

Write your content here. You can use:

- **Bold text** for emphasis
- _Italic text_ for subtle emphasis
- `Code snippets` for technical terms
- Links like [this](https://example.com)

### Subsection

More content...

## Section 2

### Lists work great:

- Point one
- Point two
- Point three

### Or numbered lists:

1. First step
2. Second step
3. Third step

## Conclusion

Wrap up your post here!

---

_Happy gaming!_  
**Your Name**
```

### Step 3: Update the Index File

**This is crucial!** You must add your post to `posts/index.json`:

1. Open `posts/index.json`
2. Click the **pencil icon** to edit
3. Add your post entry to the `"posts"` array (at the top for newest first):

```json
{
  "id": "your-post-title",
  "title": "Your Amazing Post Title",
  "excerpt": "A brief description of your post (1-2 sentences that will appear on the blog listing page)",
  "author": "Your Name",
  "date": "2025-01-20",
  "tags": ["tag1", "tag2", "tag3"],
  "featured": false
}
```

**Important Notes:**

- `"id"` must match your filename (without .md)
- `"date"` format: YYYY-MM-DD
- `"featured": true` makes the post appear prominently
- Keep `"excerpt"` under 200 characters

### Step 4: Commit Your Changes

1. Scroll down to **"Commit changes"**
2. Add a commit message like: `Add new blog post: Your Post Title`
3. Click **"Commit changes"**

🎉 **That's it!** Your post will appear on the website within a few minutes.

## 📝 Writing Guidelines

### Post Structure

- **Title**: Clear and descriptive (will appear as H1)
- **Introduction**: Hook the reader in the first paragraph
- **Body**: Use headers (##, ###) to break up sections
- **Conclusion**: Wrap up with next steps or call-to-action

### Tone & Style

- **Conversational**: Write like you're talking to a friend
- **Enthusiastic**: Share your excitement about game development
- **Inclusive**: Use "we" and "our" to include the community
- **Professional**: Maintain quality while being approachable

### Content Ideas

- Development updates and progress
- Behind-the-scenes insights
- Technical deep-dives
- Team member spotlights
- Community features and feedback
- Game design philosophy
- Challenges and solutions
- Milestone celebrations

## 🖼️ Adding Images (Optional)

### Step 1: Upload Image

1. Go to the `images/` folder
2. Click **"Add file"** → **"Upload files"**
3. Upload your image (PNG, JPG, or GIF)
4. Name it descriptively: `dev-update-2-screenshot.png`

### Step 2: Reference in Post

Add this to your markdown where you want the image:

```markdown
![Alt text description](https://raw.githubusercontent.com/YOUR-USERNAME/cri-smile-blog-content/main/images/your-image.png)
```

Replace `YOUR-USERNAME` with the actual GitHub username.

## 📋 Quick Reference

### Markdown Cheat Sheet

| Element         | Syntax        |
| --------------- | ------------- |
| Heading 1       | `# H1`        |
| Heading 2       | `## H2`       |
| Heading 3       | `### H3`      |
| Bold            | `**bold**`    |
| Italic          | `*italic*`    |
| Code            | `` `code` ``  |
| Link            | `[text](url)` |
| List            | `- item`      |
| Numbered        | `1. item`     |
| Quote           | `> quote`     |
| Horizontal Line | `---`         |

### Common Tags

- `announcement`, `welcome`, `update`
- `development`, `programming`, `design`
- `art`, `music`, `sound`
- `team`, `spotlight`, `interview`
- `tutorial`, `technical`, `tips`
- `community`, `feedback`, `testing`
- `milestone`, `release`, `launch`

## ❗ Important Rules

### ✅ DO:

- Write engaging, valuable content
- Use proper grammar and spelling
- Test links before publishing
- Keep excerpts concise but descriptive
- Use descriptive file names
- Update index.json for every new post

### ❌ DON'T:

- Forget to update index.json (post won't appear!)
- Use spaces in file names (use hyphens instead)
- Make excerpts too long (breaks layout)
- Upload very large images (keep under 2MB)
- Use special characters in post IDs

## 🆘 Troubleshooting

### My post doesn't appear on the website

- Check that you updated `posts/index.json`
- Verify the `"id"` matches your filename exactly
- Ensure the JSON syntax is valid (no missing commas/quotes)

### I made a mistake in my post

- Edit the `.md` file directly on GitHub
- Click the pencil icon, make changes, commit

### I want to delete a post

- Delete the `.md` file
- Remove the entry from `index.json`
- Commit the changes

### The website shows an error

- Check the browser console for details
- Verify all JSON syntax in `index.json`
- Make sure the repository is public

## 🚀 Advanced Features

### Code Blocks

For multi-line code:

````markdown
```javascript
function hello() {
  console.log("Hello, world!");
}
```
````

### Blockquotes

For important callouts:

```markdown
> "This is an important quote or callout that will stand out from the rest of the text."
```

### Tables

For structured data:

```markdown
| Feature | Status         | Notes              |
| ------- | -------------- | ------------------ |
| Physics | ✅ Done        | Working well       |
| Audio   | 🔄 In Progress | 80% complete       |
| UI      | 📅 Planned     | Starting next week |
```

## 📞 Need Help?

- **Questions about content?** Ask in our team chat
- **Technical issues?** Check the troubleshooting section above
- **Want to suggest improvements?** Open an issue in this repository

---

**Happy blogging!** 🎮✨

_Last updated: January 2025_
