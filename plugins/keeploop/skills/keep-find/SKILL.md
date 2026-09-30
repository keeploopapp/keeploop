---
name: keep-find
description: "Find a file someone sent you by describing it, then read the best match."
disable-model-invocation: true
---

Use the Keeploop tools from whichever Keeploop connector this chat has: the Keeploop extension in the Claude app on my Mac, or Keeploop Remote on the web and phone. If both are there, use the extension. Their names may carry a prefix; use them by their Keeploop name. If no Keeploop connector is available, tell me to turn on the Keeploop extension or Keeploop Remote, and stop.

Find an email attachment for me, using the Keeploop tools.
What I am looking for: (the text I typed after the command)
(If that is empty, ask me for it before calling any tool.)

1. Call find_attachments. Pull a filename word into query, a sender into sender, and the file type into kind (pdf, image, doc, sheet, or any). If nothing matches, retry with fewer filters.
2. Pick the best match and call read_attachment with its mail_id and attachment_id.
Then tell me which file it is (name, sender, date, mail_id) and what it says in a few lines. List up to three other candidates. Call save_attachment only if I ask for the file itself.
If a tool is missing, or answers that it needs Keeploop Pro, say so in one line and do what you can with search_mail and get_email instead.
