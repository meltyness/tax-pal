# tax-pal
Sometimes, you forgot the syntax or something. This can help you come up with more guesses faster.

# Installation
Configure ollama on your local machine:
- https://ollama.com/blog/ollama-is-now-available-as-an-official-docker-image
> [!INFO]
> If you don't use a GPU, you'll need to amend the `ollama` script.

Import the `ollama` script into your path.

Make a keyboard shortcut in your window manager to pop up a tiny dialog.
```bash
xfce4-terminal --geometry=45x10 --hide-scrollbar --hide-toolbar --hide-menubar -x ollama run gemma3:pair
```

Where `gemma3:pair` is a Modelfile like
```docker
FROM gemma3
SYSTEM "Be extremely concise. This is an excerpt of a brief informal message between pair programmers."
```

Here's kind of how that looks:
![image](https://github.com/user-attachments/assets/e91571c2-6896-4786-9a36-6d9f779512f9)
