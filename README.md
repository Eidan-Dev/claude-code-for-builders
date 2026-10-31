mkdir claude-code-for-builders && cd claude-code-for-builders
mkdir -p .claude/commands examples

cat > CLAUDE.md <<'EOF'
# CLAUDE.md - My Builder Setup
You are my co-builder, not just a coder. You help me SHIP fast.

<img width="1016" height="641" alt="Capture d&#39;écran 2026-10-30 214158" src="https://github.com/user-attachments/assets/b13097f3-4e81-4e4d-9f85-e402a1c0f603" />

## Who I am
- I build in public on X, 1 product/week
- Stack: Python, CLI tools, simple is better
- Goal: Ship, get stars, get users.

## Rules
1. README first, code second.
2. Every product needs: 10-sec install, demo GIF, tweet hook
3. No bullshit features. MVP < 2h.

## Workflow
Idea -> /idea (5 sec) -> If >21/30 -> /ship (2h) -> /tweet -> Push 21h + Tweet 18h45
EOF

<img width="1919" height="430" alt="Capture d&#39;écran 2026-10-30 214517" src="https://github.com/user-attachments/assets/149c2368-4a8f-4ee4-9a22-1affed4ba997" />


cat > .claude/commands/ship.md <<'EOF'
/ship "idea" -> Takes raw idea to shippable repo + README + tweet in 2h. <150 lines.
EOF

cat > .claude/commands/idea.md <<'EOF'
Score: Pain/10, Market/10, Build/10. TOTAL >21/30 = SHIP else KILL. Be brutal.
EOF

cat > .claude/commands/tweet.md <<'EOF'
Template: "I wasted X doing Y. So I built Z - does ... in 5 sec. Before/After. Try it 👇" No link in main tweet.
EOF

cat > README.md <<'EOF'
# claude-code-for-builders
> The exact Claude Code setup I use to ship 1 product/week.

**Last ships:** [TidyFiles](https://github.com/Eidan-Dev/TidyFiles) + [IdeaScore](https://github.com/Eidan-Dev/IdeaScore)

## The 3 Commands
- `/ship "idea"` -> repo + README + tweet in 2h
- `/idea "idea"` -> brutal score 0-30
- `/tweet product` -> viral tweet 18h45

## Workflow
Raw Idea -> /idea -> If >21/30 -> /ship -> /tweet -> Push 21h + Tweet 18h45

Copy CLAUDE.md and .claude/ to your project and start shipping.
EOF

git init && git add . && git commit -m "feat: v1.0 - my real claude code builder setup" && git branch -M main && git remote add origin https://github.com/Eidan-Dev/claude-code-for-builders.git && git push -u origin main<img width="1016" height="641" alt="Capture d&#39;écran 2026-10-30 214158" src="https://github.com/user-attachments/assets/646593b9-25fd-4b60-963b-3b7587dfd402" />
