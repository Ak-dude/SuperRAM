SUPERRAM CLI Commands
=================

--- Project & Environment Management ---
ram init [project-name] --lang [language]           # Create new project scaffold
ram env create [env-name] --python|node|go        # Create virtual environment
ram env activate [env-name]                        # Activate environment
ram env list                                      # List all environments
ram deps install                                  # Install dependencies
ram deps update                                   # Update dependencies
ram config generate [type]                        # Generate config files (.env, .gitignore, etc.)

--- Build & Run Tools ---
ram run [script-name]                             # Run project script
ram build                                         # Build/compile project
ram start                                         # Start project services (API, DB, frontend)
ram stop                                          # Stop project services
ram restart                                       # Restart project services

--- Monitoring & Logs ---
ram logs [service] --tail                          # Tail logs for a service
ram monitor                                      # Show CPU, memory, disk usage
ram errors [log-file]                             # Parse logs for errors and highlight them

--- Git & Version Control ---
ram git status                                    # Show git status
ram git commit -m "message"                       # Commit changes
ram git push [branch]                             # Push changes to remote
ram git pull                                      # Pull latest changes
ram git branch                                    # List/manage branches
ram git clone [url]                               # Clone repository

--- Testing & Debugging ---
ram test [unit|integration]                       # Run tests
ram coverage                                      # Show code coverage in terminal
ram debug [script]                                # Launch debugger or attach to process

--- Networking & APIs ---
ram server start [port]                           # Start local development server
ram server stop                                   # Stop the server
ram api request GET|POST [url] --data [json]     # Send API requests from CLI
ram check [service]                               # Ping/check service (DB, API, etc.)

--- Automation & Utilities ---
ram schedule [command] --interval [time]         # Schedule commands to run periodically
ram snippet save [name] --content "[code]"       # Save code snippet or CLI output
ram snippet list                                  # List saved snippets
ram search [pattern] [directory]                 # Search files with regex
ram replace [pattern] [replacement] [directory]  # Search & replace across files

--- Productivity Enhancements ---
ram dashboard                                     # Show project status, running services, git status
ram alias add [shortcut] "[command]"             # Add a custom command alias
ram alias list                                    # List all aliases
ram guide                                         # Interactive prompts for common tasks
