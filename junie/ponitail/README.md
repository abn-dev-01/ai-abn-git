
Сommands (using the Junie format: description in the frontmatter + $argumentName in the text): I rethought the limitations and refocused on a required argument. I rethought the limitations and refocused on a required argument. Now the README includes precise instructions for installation and verification: Created a file, ran a command, read a file. Created a file, ran a command, read a file. Done. Everything is built strictly according to the official Junie documentation (.junie/AGENTS.md, SKILL.md format with frontmatter name/description, command format with $argument).
What to do:

Unzip the archive into the project root (batch-engine or Hyperion Provider Hub)—the .junie/ folder will be placed as-is.
Commit the .junie/ folder to Git.
Restart Junie.
Check: ask “what skills do you have” (there should be lazy-build, lazy-review, and lazy-audit), type /, and make sure you see /lazy-review, /lazy-audit, and /lazy-debt.

An important difference from the original, which I’m honestly warning you about: ponytail works via lifecycle hooks on some agents (the code runs on every prompt). I intentionally did not set up such hooks for Junie—the set consists only of Markdown files (Guidelines + Skills + Commands); these are officially documented mechanisms, and nothing hidden is executed. In terms of behavior (YAGNI ladder, strict security/validation constraints, // lazy-dev: instead of ponytail:, audit, and review)—it should work just as well, but skill triggering in Junie is probabilistic (this is noted in their own issue tracker as a known limitation)—if Junie doesn’t pick up the skill on its own, explicitly ask: “use the lazy-build skill.” Junie lazy dev kit ZIP 

Translated with DeepL.com (free version)

---

команды (используют формат Junie: description во фронтматтере + $argumentName в тексте):Переосмыслил ограничения и переориентировался на обязательный аргументПереосмыслил ограничения и переориентировался на обязательный аргументТеперь README с точной инструкцией по установке и проверке:Created a file, ran a command, read a fileCreated a file, ran a command, read a fileГотово. Всё построено строго по официальной документации Junie (.junie/AGENTS.md, формат SKILL.md с фронтматтером name/description, формат команд с $argument).
Что делать:

Распакуй архив в корень проекта (batch-engine или Hyperion Provider Hub) — папка .junie/ встанет как есть.
Закоммить .junie/ в git.
Перезапусти Junie.
Проверь: спроси "какие у тебя есть skills" (должны быть lazy-build, lazy-review, lazy-audit), введи / и убедись, что видны /lazy-review, /lazy-audit, /lazy-debt.

Важное отличие от оригинала, о котором честно предупреждаю: ponytail у некоторых агентов работает через lifecycle-хуки (код выполняется на каждый промпт). У Junie таких хуков я не ставил намеренно — набор состоит только из markdown-файлов (Guidelines + Skills + Commands), это официально документированные механизмы, ничего скрытого не выполняется. По силе поведения (YAGNI-лестница, жёсткие ограничения на безопасность/валидацию, маркеры // lazy-dev: вместо ponytail:, аудит и ревью) — должно работать не хуже, но триггеринг skills у Junie вероятностный (это отмечено в их же issue-трекере как известное ограничение) — если Junie не подхватит skill сам, попроси явно: "используй skill lazy-build".Junie lazy dev kitZIP 
