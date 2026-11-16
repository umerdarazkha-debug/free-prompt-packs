# 5 Claude Code shortcuts nobody uses

From Umer does AI. Checked against Claude Code v2.1.280.

## 1. Plan mode: Shift+Tab
Press **Shift+Tab** until the bottom line says **⏸ plan mode on**. Claude reads your files and writes a plan, but doesn't change anything until you choose **Yes**. Use it for anything bigger than a one-line fix.
> Try: "redesign my pricing page. Plan only, list every file you'd touch and what could break."

## 2. /compact
When the chat gets long, or you see "Context low", type **/compact**. It frees up context by summarizing the conversation so far. Add what to keep after it:
> /compact keep the pricing decisions and the list of files we changed

## 3. Memory: CLAUDE.md
Rules you put in **CLAUDE.md** are read at the start of every session, so you stop repeating yourself. Type **/memory** to edit them, or just ask:
> remember: captions in UK English, no emojis, never more than 2 hashtags

## 4. Skills
A skill is a folder with a **SKILL.md** file that holds your steps. Save it once, then type **/** and run it whenever you like. Claude can also pick it up on its own when the job fits.
> Turn what we just did into a skill called reel-captions so I can run it with /reel-captions

## 5. /schedule
**/schedule** creates scheduled remote Claude Code agents (routines). They run in the cloud on a repeat, so your laptop can be closed.
> /schedule every Monday 9am: check these 3 competitor pricing pages and tell me what changed

Save this. Follow @umer.does.ai for more.
