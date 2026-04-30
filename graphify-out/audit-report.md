# Graph Report - .  (2026-04-10)

## Corpus Check
- Large corpus: 1309 files · ~2,166,622 words. Semantic extraction will be expensive (many Claude tokens). Consider running on a subfolder, or use --no-semantic to run AST-only.

## Summary
- 28216 nodes · 64072 edges · 687 communities detected
- Extraction: 59% EXTRACTED · 41% INFERRED · 0% AMBIGUOUS · INFERRED: 26501 edges (avg confidence: 0.5)
- Token cost: 0 input · 0 output

## God Nodes (most connected - your core abstractions)
1. `Platform` - 2488 edges
2. `PlatformConfig` - 2152 edges
3. `MessageEvent` - 1414 edges
4. `MessageType` - 1298 edges
5. `SendResult` - 1159 edges
6. `BasePlatformAdapter` - 1091 edges
7. `AIAgent` - 1021 edges
8. `GatewayConfig` - 879 edges
9. `SessionDB` - 761 edges
10. `SessionSource` - 754 edges
11. `GatewayRunner` - 664 edges
12. `DiscordAdapter` - 459 edges
13. `HermesCLI` - 428 edges
14. `TelegramAdapter` - 414 edges
15. `SlackAdapter` - 363 edges

## Surprising Connections (you probably didn't know these)
- `run_agent_safewriter` --uses--> `todo_tool_todostore`  [EXTRACTED]
   → 
- `run_agent_iterationbudget` --uses--> `todo_tool_todostore`  [EXTRACTED]
   → 
- `run_agent_aiagent` --uses--> `error_classifier_failoverreason`  [EXTRACTED]
   → 
- `run_agent_aiagent` --uses--> `context_compressor_contextcompressor`  [EXTRACTED]
   → 
- `run_agent_aiagent` --uses--> `subdirectory_hints_subdirectoryhinttracker`  [EXTRACTED]
   → 
- `run_agent_aiagent` --uses--> `display_kawaiispinner`  [EXTRACTED]
   → 
- `run_agent_aiagent` --uses--> `checkpoint_manager_checkpointmanager`  [EXTRACTED]
   → 
- `run_agent_aiagent` --uses--> `memory_tool_memorystore`  [EXTRACTED]
   → 

## Hyperedges (group relationships)
- **RL Training Pipeline** — rl_training, trajectory_generation, atropos_environments [EXTRACTED 1.00]
- **Messaging Infrastructure** — messaging_gateway, platform_adapter, telegram_bot [EXTRACTED 1.00]
- **Honcho Memory Integration Patterns** — async_prefetch_pattern, per_peer_memory_modes, ai_peer_identity_formation [EXTRACTED 1.00]
- **blackbox tags** — coding_agent_tag, blackbox_tag, multi_agent_tag, judge_tag, multi_model_tag [EXTRACTED 0.95]
- **honcho tags** — honcho_tag, memory_tag, profiles_tag, observation_tag, dialectic_tag, user_modeling_tag [EXTRACTED 0.95]
- **base tags** — base_tag, blockchain_tag, crypto_tag, web3_tag, rpc_tag, de_fi_tag, evm_tag, l2_tag, ethereum_tag [EXTRACTED 0.95]
- **solana tags** — solana_tag, blockchain_tag, crypto_tag, web3_tag, rpc_tag, de_fi_tag, nft_tag [EXTRACTED 0.95]
- **one-three-one-rule tags** — communication_tag, decision_making_tag, proposals_tag, trade_offs_tag [EXTRACTED 0.95]
- **blender-mcp tags** — blender_tag, 3d_tag, animation_tag, modeling_tag, bpy_tag, mcp_tag [EXTRACTED 0.95]
- **meme-generation tags** — creative_tag, memes_tag, humor_tag, images_tag [EXTRACTED 0.95]
- **inference-sh-cli tags** — ai_tag, image_generation_tag, video_tag, llm_tag, search_tag, inference_tag, flux_tag, veo_tag, claude_tag [EXTRACTED 0.95]
- **docker-management tags** — docker_tag, containers_tag, devops_tag, infrastructure_tag, compose_tag, images_tag, volumes_tag, networks_tag, debugging_tag [EXTRACTED 0.95]
- **agentmail tags** — email_tag, communication_tag, agentmail_tag, mcp_tag [EXTRACTED 0.95]
- **neuroskill-bci tags** — bci_tag, neurofeedback_tag, health_tag, focus_tag, eeg_tag, cognitive_state_tag, biometrics_tag, neuroskill_tag [EXTRACTED 0.95]
- **Ai Agent Skills** — blackbox_skill, hermes_agent_skill, honcho_skill, agentmail_skill [INFERRED 0.80]
- **Hermes Optional Skills** — blackbox_skill, claude_code_skill, codex_skill, hermes_agent_skill, honcho_skill [EXTRACTED 0.90]
- **LLM Data Extraction & Curation Pipeline** —  [INFERRED]
- **GPU-Accelerated ML Stack** —  [INFERRED]
- **Multi-Provider LLM Support** —  [INFERRED]
- **he_19** — simpo_preference_optimization, simpo_alignment, simpo_training_workflow [EXTRACTED 1.00]
- **he_20** — saelens_sparse_autoencoder, saelens_feature_discovery, saelens_mechanistic_interpretability [EXTRACTED 1.00]
- **Memory Provider Ecosystem** — memory_openviking, memory_retaindb, memory_supermemory, memory_byterover, memory_hindsight, memory_holographic, memory_honcho, memory_mem0 [EXTRACTED 1.00]
- **Semantic Search Techniques** — semantic_search, memory_retaindb, memory_supermemory, memory_hindsight, memory_holographic [INFERRED 0.85]
- **Provider Authentication Strategy** — plan_gemini_oauth, oauth_standard, ai_provider_ecosystem [INFERRED 0.75]
- **he_24** —  [INFERRED]
- **he_25** —  [INFERRED]
- **he_26** —  [INFERRED]
- **github_workflow** — github_auth_skill, github_code_review_skill, codebase_inspection_skill [INFERRED 0.70]
- **he_28** — guidance_constrained_generation, outlines_structured_generation, vllm_high_throughput [INFERRED 0.80]
- **he_29** — gguf_quantization, llama_cpp_inference, hardware_acceleration [INFERRED 0.85]
- **he_30** — obliteratus_abliteration, mechanistic_interpretability, outlines_structured_generation [INFERRED 0.70]
- **he_31** — audiocraft_musicgen, audiocraft_style_generation, audiocraft_melody_conditioning [INFERRED 0.80]
- **he_32** — stable_diffusion_t2i, stable_diffusion_controlnet, stable_diffusion_lora [INFERRED 0.80]
- **he_33** — audiocraft_troubleshooting, stable_diffusion_troubleshooting, cuda_optimization [INFERRED 0.75]
- **Google Workspace Integrated Services** — google_workspace_gmail, google_workspace_calendar, google_workspace_drive, google_workspace_sheets, google_workspace_docs [EXTRACTED 1.00]
- **Research Paper Writing Workflow** — experiment-patterns_research, human-evaluation_research, citation-workflow_research, checklists_research, reviewer-guidelines_research [INFERRED 0.80]
- **Conference Submission Requirements** — neurips_venue, icml_venue, acl_venue, checklists_research [EXTRACTED 0.95]
- **Citation Verification Infrastructure** — semantic-scholar_api, crossref_api, citation-workflow_research, citation-hallucination_concept [INFERRED 0.85]
- **he_38** — writing_plans_skill, subagent_driven_development_skill, requesting_code_review_skill [INFERRED 0.85]
- **he_39** — tdd_skill, systematic_debugging_skill, requesting_code_review_skill [INFERRED 0.80]
- **he_40** — xitter_skill, x_api_credentials, x_cli_client [INFERRED 0.90]
- **Agent Core Architecture** — agent_loop_doc, tools_runtime_doc, acp_doc [EXTRACTED 0.95]
- **Extensibility Mechanisms** — add_tools_doc, create_skills_doc, mem_provider_doc, plugins_doc [EXTRACTED 0.90]
- **Deployment & Integration** — gateway_doc, quickstart_doc, mcp_guide_doc, cron_doc [INFERRED 0.80]
- **he_44** — mcp_protocol, mcp_servers_config, tools_and_toolsets [INFERRED]
- **he_45** — delegation_patterns, parallel_research, code_review_delegation, multi_file_refactoring [INFERRED]
- **he_46** — skills_system, skill_md_format, conditional_skill_activation, skills_hub [INFERRED]
- **Voice Integration Across Messaging Platforms** — voice_feature, telegram_messaging, discord_messaging, slack_messaging [INFERRED 0.80]
- **Team Communication Messaging Platforms** — telegram_messaging, discord_messaging, slack_messaging, mattermost_messaging [INFERRED 0.85]
- **Core Agent Features** — hermes_search_feature, session_recap_feature, tool_output_feature, subagent_delegation_feature [INFERRED 0.70]

## Communities

### Community 0 - "Platform / PlatformConfig"
Cohesion: 0.0
Nodes (2571): Hermes Agent API Server, APIServerAdapter, body_limit_middleware(), check_api_server_requirements(), cors_middleware(), _extract_output_items(), _IdempotencyCache, _make_request_fingerprint() (+2563 more)

### Community 1 - "AIAgent / SessionDB"
Cohesion: 0.0
Nodes (1602): AuthError, Structured auth error with UX mapping hints., AutoSuggest, BatchRunner, _extract_reasoning_stats(), _extract_tool_stats(), main(), _normalize_tool_error_counts() (+1594 more)

### Community 2 - "ContextCompressor / CheckpointManager"
Cohesion: 0.0
Nodes (776): BuiltinMemoryProvider, BuiltinMemoryProvider — wraps MEMORY.md / USER.md as a MemoryProvider.  Always r, Access the underlying MemoryStore for legacy code paths., Built-in file-backed memory (MEMORY.md + USER.md).      Always active, never dis, Built-in memory is always available., Load memory from disk if not already loaded., Return MEMORY.md and USER.md content for the system prompt.          Uses the fr, Built-in memory doesn't do query-based recall — it's injected via system_prompt_ (+768 more)

### Community 3 - "LocalEnvironment / BaseEnvironment"
Cohesion: 0.01
Nodes (469): BaseEnvironment, cache_audio_from_bytes(), cache_audio_from_url(), cache_document_from_bytes(), cache_image_from_bytes(), cache_image_from_url(), cleanup(), cleanup_document_cache() (+461 more)

### Community 4 - "ToolRegistry / MCPServerTask"
Cohesion: 0.01
Nodes (283): _build_safe_env(), _build_utility_schemas(), _check_message_handler_support(), _connect_server(), _convert_mcp_schema(), _discover_and_register_server(), discover_mcp_tools(), _ensure_mcp_loop() (+275 more)

### Community 5 - "ScanResult / Skills Hub - Multi-Source"
Cohesion: 0.01
Nodes (286): CLI Interface & Commands, Conditional Skill Activation & Fallbacks, MEMORY.md - Agent Personal Notes, External Memory Provider Plugins, Persistent Memory System, Hermes Profiles System, Session Search & Recall, SKILL.md Format & Metadata (+278 more)

### Community 6 - "HonchoSessionManager / SessionManager"
Cohesion: 0.01
Nodes (214): _active_profile_name(), _all_profile_host_configs(), clone_honcho_for_profile(), cmd_disable(), cmd_enable(), cmd_identity(), cmd_map(), cmd_migrate() (+206 more)

### Community 7 - "hermes_constants.py / tirith_security.py"
Cohesion: 0.01
Nodes (402): _api_key_default_label(), auth_add_command(), auth_command(), auth_list_command(), auth_remove_command(), auth_reset_command(), _display_source(), _format_exhausted_status() (+394 more)

### Community 8 - "HermesAgentLoop / AgentResult"
Cohesion: 0.01
Nodes (280): HermesAgentLoop, AgentResult, _extract_reasoning_from_message(), HermesAgentLoop, HermesAgentLoop -- Reusable Multi-Turn Agent Engine  Runs the hermes-agent tool-, Runs hermes-agent's tool-calling loop using standard OpenAI-spec tool calling., Initialize the agent loop.          Args:             server: Server object with, Execute the full agent loop using standard OpenAI tool calling.          Args: (+272 more)

### Community 9 - "CodexAuxiliaryClient / AnthropicAuxiliaryClient"
Cohesion: 0.01
Nodes (223): AnthropicAuxiliaryClient, _AnthropicChatShim, _AnthropicCompletionsAdapter, async_call_llm(), AsyncAnthropicAuxiliaryClient, _AsyncAnthropicChatShim, _AsyncAnthropicCompletionsAdapter, AsyncCodexAuxiliaryClient (+215 more)

### Community 10 - "__init__.py / MemoryStore"
Cohesion: 0.01
Nodes (165): DeepSeekV31ToolCallParser, DeepSeek V3.1 tool call parser.  Similar to V3 but with a slightly different for, Parser for DeepSeek V3.1 tool calls.      Slightly different regex than V3: func, DeepSeekV3ToolCallParser, DeepSeek V3 tool call parser.  Format uses special unicode tokens:     <｜tool▁ca, Parser for DeepSeek V3 tool calls.      Uses special unicode tokens with fullwid, Parses the input text and extracts all available tool calls., _deserialize_value() (+157 more)

### Community 11 - "ShellFileOperations / PatchResult"
Cohesion: 0.01
Nodes (156): ABC, ExecuteResult, FileOperations, _get_safe_write_root(), _is_write_denied(), LintResult, PatchResult, Return True if path is on the write deny list. (+148 more)

### Community 12 - "model_tools.py / TestCoerceToolArgs"
Cohesion: 0.01
Nodes (112): check_tool_availability(), check_toolset_requirements(), _coerce_boolean(), _coerce_number(), coerce_tool_args(), _coerce_value(), _discover_tools(), get_all_tool_names() (+104 more)

### Community 13 - "ProcessRegistry / ProcessSession"
Cohesion: 0.01
Nodes (124): build_execute_code_schema(), check_sandbox_requirements(), _env_temp_dir(), execute_code(), _execute_remote(), generate_hermes_tools_module(), _get_or_create_env(), _kill_process_group() (+116 more)

### Community 14 - "NousSubscriptionFeatures / NousFeatureState"
Cohesion: 0.02
Nodes (81): apply_nous_managed_defaults(), apply_nous_provider_defaults(), _browser_label(), get_nous_subscription_features(), _has_agent_browser(), _model_config_dict(), NousFeatureState, NousSubscriptionFeatures (+73 more)

### Community 15 - "DirectAlias / ModelSwitchResult"
Cohesion: 0.02
Nodes (137): _check_hermes_model_warning(), CustomAutoResult, DirectAlias, _ensure_direct_aliases(), get_authenticated_provider_slugs(), list_authenticated_providers(), _load_direct_aliases(), ModelIdentity (+129 more)

### Community 16 - "TestConvertMessages / test_anthropic_adapter.py"
Cohesion: 0.01
Nodes (53): Tests for agent/anthropic_adapter.py — Anthropic Messages API adapter., Date-stamped model IDs should resolve via substring match., Unknown future models should get the highest known limit., User-specified max_tokens should be respected., max_tokens should be clamped to context_length if it's smaller., No clamping when context_length exceeds output limit., claude-3-5-sonnet' should match before 'claude-3-5'., Circular dict reference should be stringified, not infinite-loop. (+45 more)

### Community 17 - "prompt_builder.py / transcription_tools.py"
Cohesion: 0.02
Nodes (139): build_channel_directory(), _build_discord(), _build_from_sessions(), _build_slack(), _channel_target_name(), format_directory_for_display(), load_directory(), _normalize_channel_query() (+131 more)

### Community 18 - "DebugSession / web_tools.py"
Cohesion: 0.02
Nodes (144): DebugSession, Per-tool debug session that records tool calls to a JSON log file.      Activate, Append a tool-call entry to the in-memory log., Flush the in-memory log to a JSON file in the logs directory., Return a summary dict suitable for returning from get_debug_session_info()., check_fal_api_key(), check_image_generation_requirements(), get_debug_session_info() (+136 more)

### Community 19 - "PluginManager / PluginContext"
Cohesion: 0.03
Nodes (109): discover_plugins(), _env_enabled(), _get_disabled_plugins(), get_plugin_cli_commands(), get_plugin_manager(), get_plugin_tool_names(), get_plugin_toolsets(), invoke_hook() (+101 more)

### Community 20 - "test_voice_command.py / _make_receiver()"
Cohesion: 0.02
Nodes (65): TestOpusFindLibrary, adapter(), _build_rtp_packet(), _ensure_discord_mock(), _fill_buffer(), _make_discord_adapter(), _make_event(), _make_receiver() (+57 more)

### Community 21 - "telephony.py / HermesTokenStorage"
Cohesion: 0.03
Nodes (113): build_oauth_auth(), _can_open_browser(), _find_free_port(), _get_token_dir(), HermesTokenStorage, _is_interactive(), _make_callback_handler(), OAuthNonInteractiveError (+105 more)

### Community 22 - "EventBridge / QueueEvent"
Cohesion: 0.02
Nodes (69): create_mcp_server(), EventBridge, _extract_attachments(), _extract_message_content(), _get_session_db(), _get_sessions_dir(), _load_channel_directory(), _load_sessions_index() (+61 more)

### Community 23 - "test_approval.py / TestNormalizationBypass"
Cohesion: 0.01
Nodes (59): Tests for the dangerous command approval module., Regression tests: filenames starting with 'r' must NOT trigger recursive delete., Ensure all recursive delete flag styles are still caught., Newlines in commands must not bypass dangerous pattern detection., Detect remote code execution via process substitution., Detect tee writes to sensitive system files., Detect find -exec with full-path rm bypasses., Detect shell redirection writes to sensitive user-managed paths. (+51 more)

### Community 24 - "ProviderConfig / TestResolveProvider"
Cohesion: 0.02
Nodes (41): ProviderConfig, Describes a known inference provider., Tests for API-key provider support (z.ai/GLM, Kimi, MiniMax, AI Gateway)., Ensure we didn't break the existing OAuth providers., Test resolve_provider() with new providers., OpenRouter API key should win over GLM in auto-detection., ZAI_API_KEY should work when GLM_API_KEY is not set., Test that new providers are correctly registered. (+33 more)

### Community 25 - "AudioRecorder / TermuxAudioRecorder"
Cohesion: 0.02
Nodes (80): mock_sd(), Tests for tools.voice_mode -- all mocked, no real microphone or API calls., Verify current_rms property updates in real-time for UI feedback., Verify that silence detection params can be configured., Bug: proc.wait(timeout) raised TimeoutExpired but process was not killed., WSL with PULSE_SERVER set should NOT block voice mode., Bug: stream.start() failure left stream unclosed., Bug: _on_silence_stop was read/written without lock in audio callback. (+72 more)

### Community 26 - "TrajectoryCompressor / CompressionConfig"
Cohesion: 0.02
Nodes (86): _count_tokens_for_entry(), _init_tokenizer_worker(), load_dataset_from_hf(), main(), merge_output_to_single_jsonl(), Load all datasets, filter by token count, then randomly sample from combined poo, Save samples to JSONL files for trajectory compression.          Args:         s, Run trajectory compression on the sampled data.          Args:         input_dir (+78 more)

### Community 27 - "config.py / ConfigIssue"
Cohesion: 0.03
Nodes (118): _apply_env_overrides(), check_config_version(), _coerce_bool(), config_command(), ConfigIssue, _deep_merge(), edit_config(), _ensure_default_soul_md() (+110 more)

### Community 28 - "CloudBrowserProvider / BrowserUseProvider"
Cohesion: 0.05
Nodes (108): CloudBrowserProvider, Interface for cloud browser backends (Browserbase, Steel, etc.).      Implementa, _allow_private_urls(), browser_back(), _browser_cleanup_thread_worker(), browser_click(), browser_console(), _browser_eval() (+100 more)

### Community 29 - "auth.py / _load_auth_store()"
Cohesion: 0.03
Nodes (131): _agent_key_is_usable(), _auth_file_path(), _auth_lock_path(), _auth_store_lock(), clear_provider_auth(), _codex_access_token_is_expiring(), _codex_device_code_login(), _coerce_ttl_seconds() (+123 more)

### Community 30 - "test_slack.py / TestFormatMessage"
Cohesion: 0.02
Nodes (11): _ensure_slack_mock(), _redirect_cache(), test_document_download_error_handled(), test_image_still_handled(), test_large_txt_not_injected(), test_md_document_injects_content(), test_oversized_document_skipped(), test_pdf_document_cached() (+3 more)

### Community 31 - "test_transcription_tools. / TestTranscribeAudioDispat"
Cohesion: 0.02
Nodes (46): clean_env(), mock_mistral_module(), Tests for tools.transcription_tools — three-provider STT pipeline.  Covers the f, Explicit openai with no key returns none — no cross-provider fallback., When stt.provider is explicitly set, that choice is authoritative.     No silent, GH-1774: provider=local must not silently fall back to openai         even when, Local-to-local_command fallback is fine — both are local., When no provider is explicitly set, auto-detect cloud fallback works. (+38 more)

### Community 32 - "test_profiles.py / TestExportImport"
Cohesion: 0.02
Nodes (48): profile_env(), Comprehensive tests for hermes_cli.profiles module.  Tests cover: validation, di, Tests for create_profile()., Clone config gracefully skips files that don't exist in source., Tests for delete_profile()., Tests for list_profiles()., Tests for set_active_profile() / get_active_profile()., Tests for get_active_profile_name(). (+40 more)

### Community 33 - "jobs.py / load_jobs()"
Cohesion: 0.02
Nodes (88): get_timezone(), get_timezone_name(), _get_zoneinfo(), now(), Timezone-aware clock for Hermes.  Provides a single ``now()`` helper that return, Return the current time as a timezone-aware datetime.      If a valid timezone i, Clear the cached timezone. Used by tests and after config changes., Read the configured IANA timezone string (or empty string).      This does file (+80 more)

### Community 34 - "TestExecuteCode / ._run()"
Cohesion: 0.02
Nodes (53): _force_local_terminal(), _mock_handle_function_call(), Verify json_parse, shell_quote, and retry helpers are generated., Integration tests using the mock dispatcher., Helper: run code with mocked handle_function_call., Script that just prints -- no tool calls., Sandboxed scripts can import modules that live at the repo root., Script calls terminal and prints the result. (+45 more)

### Community 35 - "setup.py / print_info()"
Cohesion: 0.04
Nodes (118): _apply_default_agent_settings(), check_auth(), _check_espeak_ng(), _clean_discord_user_ids(), _current_reasoning_effort(), _curses_prompt_choice(), _ensure_deps(), exchange_auth_code() (+110 more)

### Community 36 - "gateway.py / gateway_command()"
Cohesion: 0.04
Nodes (105): _build_user_local_paths(), _default_system_service_user(), _detect_venv_dir(), _ensure_linger_enabled(), _ensure_user_systemd_env(), find_gateway_pids(), gateway_command(), gateway_setup() (+97 more)

### Community 37 - "Hermes Agent / test_openai_client_lifecy"
Cohesion: 0.02
Nodes (110): Access Control / User Allowlists, ACP for JetBrains, Agent Client Protocol (ACP), ACP for VS Code, ACP for Zed, AIAgent Class & Initialization, Hermes Atropos Environments, Atropos Integration (+102 more)

### Community 38 - "test_clipboard.py / TestPreprocessImagesWithV"
Cohesion: 0.02
Nodes (24): Tests for clipboard image paste — clipboard extraction, multimodal conversion, a, When both PNG and BMP are available, PNG should be preferred., Test that _linux_save dispatches correctly to WSL → Wayland → X11., Test vision-based image pre-processing for the CLI., Return an async mock that simulates a successful vision_analyze_tool call., Return an async mock that simulates a failed vision_analyze_tool call., Test the clipboard → state flow., TestHasClipboardImage (+16 more)

### Community 39 - "test_scheduler.py / TestDeliverResultWrapping"
Cohesion: 0.02
Nodes (53): Tests for cron/scheduler.py — origin resolution, delivery routing, and error log, Failed jobs deliver regardless of [SILENT] in output., Verify _build_job_prompt always injects [SILENT] guidance., deliver: 'telegram:My Group' resolves without display suffix., Cron hint tells agents their final response is auto-delivered., System guidance appears before the user's prompt text., Verify that a missing skill logs a warning and does not crash the job., Job should run even when a referenced skill is not installed. (+45 more)

### Community 40 - "test_matrix.py / _make_adapter()"
Cohesion: 0.02
Nodes (35): _make_adapter(), _make_fake_nio(), test_create_room(), test_create_room_no_client(), test_disconnect_exports_keys(), test_disconnect_handles_export_failure(), test_disconnect_skips_export_when_no_encryption(), test_expired_events_dropped() (+27 more)

### Community 41 - "test_tirith_security.py / _mock_run()"
Cohesion: 0.02
Nodes (58): _json_stdout(), _mock_run(), Tests for the tirith security scanning subprocess wrapper., Without HERMES_HOME set, falls back to ~/.hermes., Pre-set cached path to skip auto-install in scan tests.      Tests that specific, _resolve_tirith_path should expand ~ in configured path., Build a mock subprocess.CompletedProcess., ensure_installed must return immediately when download needed. (+50 more)

### Community 42 - "TestBackendSelection / TestFirecrawlClientConfig"
Cohesion: 0.02
Nodes (49): Tests for web backend client configuration and singleton behavior.  Coverage:, Shared gateway scheme should allow local plain-http vendor hosts., Unexpected shared gateway schemes should fail fast., An explicit Firecrawl gateway origin should override the shared domain., Default gateway origin should point at the Firecrawl vendor hostname., Explicit Firecrawl config should win over the gateway fallback., Auth lookup should read from HERMES_HOME/auth.json, not ~/.hermes/auth.json., Availability checks should not be pinned to module import state. (+41 more)

### Community 43 - "test_feishu.py / TestAdapterModule"
Cohesion: 0.02
Nodes (7): _mock_event_dispatcher_builder(), test_connect_acquires_scoped_lock_and_disconnect_releases_it(), test_connect_retries_transient_startup_failure(), test_connect_webhook_mode_starts_local_server(), TestAdapterBehavior, TestAdapterModule, TestWebhookSecurity

### Community 44 - "feishu.py / normalize_feishu_message("
Cohesion: 0.04
Nodes (68): _attachment_placeholder(), _build_create_message_body(), _build_create_message_request(), _build_file_upload_body(), _build_file_upload_request(), _build_get_chat_request(), _build_get_message_request(), _build_image_upload_body() (+60 more)

### Community 45 - "_make_skill() / test_skills_tool.py"
Cohesion: 0.03
Nodes (29): _make_skill(), Tests for tools/skills_tool.py — skill discovery and viewing., If no description in frontmatter, first non-header line is used., Helper to create a minimal skill directory., Disabled skills should not be viewable via skill_view., Non-disabled skills should be viewable normally., Tests for the platforms frontmatter field filtering., Skills without a platforms field should load on any OS. (+21 more)

### Community 46 - "test_api_server.py / _create_app()"
Cohesion: 0.03
Nodes (70): adapter(), auth_adapter(), _create_app(), _make_adapter(), test_agent_error_returns_500(), test_browser_origin_rejected_by_default(), test_chat_completions_requires_auth(), test_chat_completions_usage() (+62 more)

### Community 47 - "_setup_worktree() / test_worktree.py"
Cohesion: 0.03
Nodes (63): _cleanup_worktree(), git_repo(), _git_repo_root(), Tests for git worktree isolation (CLI --worktree / -w flag).  Verifies worktree, Test git repo root detection., Create a temporary git repo for testing., Two worktrees from the same repo are independent., Worktree should contain the repo's tracked files. (+55 more)

### Community 48 - "test_model_metadata.py / TestParseContextLimitFrom"
Cohesion: 0.02
Nodes (28): Tests for agent/model_metadata.py — token estimation, context lengths, probing,, Ollama model:tag format must NOT be stripped., Value above 128K should return 128K., Very large number (>10M) should be rejected., Saving a different value for the same key overwrites it., Corrupted cache file is handled gracefully., Unicode chars are still 1 Python char each — 4 chars/token holds., YAML that loads but has wrong structure. (+20 more)

### Community 49 - "TestRetainDBMemoryProvide / ._make_provider()"
Cohesion: 0.03
Nodes (20): _isolate_env(), Tests for the RetainDB memory plugin.  Covers: _Client HTTP client, _WriteQueue, Test the SQLite-backed write queue with real SQLite., Ensure HERMES_HOME and RETAINDB vars are isolated., Simulate crash: create rows, then new queue should replay them., Test the overlay formatter (pure function)., Test the main plugin class., Test the HTTP client with mocked requests. (+12 more)

### Community 50 - "test_models.py / TestFilterNousFreeModels"
Cohesion: 0.02
Nodes (45): Tests for the hermes_cli models module., Models belonging to the current provider should not trigger a switch., Models in the OpenRouter catalog should be found., Completely unknown model names should return None., nous/openrouter should never be auto-suggested as target provider., Tests for filter_nous_free_models — Nous Portal free-model policy., Regular paid models pass through unchanged., Free models NOT in the allowlist are filtered out. (+37 more)

### Community 51 - "_make_mock_parent() / test_delegate.py"
Cohesion: 0.03
Nodes (47): _make_mock_parent(), Verify child gets parent's depth + 1., Verify children are registered/unregistered for interrupt propagation., Verify _last_resolved_tool_names is restored after subagent runs., The process-global _last_resolved_tool_names must be restored         after a su, Even when the child agent raises, the global must be restored., Regression: _build_child_agent must not reference _saved_tool_names.          Th, Create a mock parent agent with the fields delegate_task expects. (+39 more)

### Community 52 - "test_gateway_service.py / TestProfileArg"
Cohesion: 0.02
Nodes (35): Tests for gateway service management helpers., Without --all, stop uses systemd (if available) and does NOT call         the gl, With --all, stop uses systemd AND calls the global kill_gateway_processes()., Exit code 113 (\"Could not find service\") should also trigger bootstrap recover, Tests for _detect_venv_dir() virtualenv detection., HERMES_HOME in system units must reference the target user, not root., Unit tests for _hermes_home_for_target_user()., ~/.local/bin must be in PATH so uvx/pipx tools are discoverable. (+27 more)

### Community 53 - "models.py / normalize_provider()"
Cohesion: 0.04
Nodes (84): check_nous_free_tier(), clear_nous_free_tier_cache(), _copilot_catalog_ids(), _copilot_catalog_item_is_text_model(), copilot_default_headers(), copilot_model_api_mode(), curated_models_for_provider(), detect_provider_for_model() (+76 more)

### Community 54 - "tools.py / events.py"
Cohesion: 0.03
Nodes (61): make_message_cb(), make_step_cb(), make_thinking_cb(), make_tool_progress_cb(), Callback factories for bridging AIAgent events to ACP notifications.  Each facto, Create a ``thinking_callback`` for AIAgent., Create a ``step_callback`` for AIAgent.      Signature expected by AIAgent::, Create a callback that streams agent response text to the editor. (+53 more)

### Community 55 - "_validate() / test_model_validation.py"
Cohesion: 0.03
Nodes (25): Tests for provider-aware `/model` validation in hermes_cli.models., custom:name:model → named custom provider., Triple syntax should handle whitespace., custom:name: with no model → treated as custom:name (bare)., GPT-5+ models should use Responses API (matching opencode)., gpt-5-mini is the exception — uses Chat Completions., Non-GPT-5 models use Chat Completions., When catalog shows both endpoints, model ID pattern wins. (+17 more)

### Community 56 - "parseltongue.py / detect_triggers()"
Cohesion: 0.02
Nodes (82): _apply_acrostic(), _apply_base64hint(), _apply_brackets(), _apply_bubble(), _apply_bubblespaced(), _apply_dotted(), _apply_dottedunicode(), _apply_fullwidth() (+74 more)

### Community 57 - "test_telegram_format.py / TestStripMdv2"
Cohesion: 0.02
Nodes (11): TestEscapeMdv2, TestFormatMessageBasic, TestFormatMessageBlockquote, TestFormatMessageBoldItalic, TestFormatMessageCodeBlocks, TestFormatMessageComplex, TestFormatMessageHeaders, TestFormatMessageLinks (+3 more)

### Community 58 - "Migrator / .record()"
Cohesion: 0.09
Nodes (25): backup_existing(), dump_yaml_file(), ensure_parent(), extract_markdown_entries(), ItemResult, load_yaml_file(), main(), merge_entries() (+17 more)

### Community 59 - "test_jobs.py / TestComputeNextRun"
Cohesion: 0.03
Nodes (24): Tests for cron/jobs.py — schedule parsing, job CRUD, and due-job detection., Redirect cron storage to a temp directory., Agent succeeds but delivery fails — both tracked independently., Successful delivery clears the previous delivery error., Agent fails AND delivery fails — both errors recorded., Tests for advance_next_run() — crash-safety for recurring jobs., Interval jobs should have next_run_at bumped to the next future occurrence., Cron-expression jobs should have next_run_at bumped to the next occurrence. (+16 more)

### Community 60 - "_make_secret_key() / _make_voice_receiver()"
Cohesion: 0.05
Nodes (50): _build_encrypted_rtp_packet(), _make_secret_key(), _make_voice_receiver(), Integration tests for Discord voice channel audio flow.  Uses real NaCl encrypti, End-to-end: real NaCl encrypt → _on_packet decrypt → buffer., Real NaCl encrypted packet → decrypted → buffered., Packet encrypted with wrong key → NaCl fails → not buffered., Packet from bot's own SSRC → ignored. (+42 more)

### Community 61 - "test_plugins_cmd.py / TestSanitizePluginName"
Cohesion: 0.03
Nodes (30): Tests for hermes_cli.plugins_cmd — the ``hermes plugins`` CLI subcommand., Extract plugin directory name from Git URLs., Verify alias routing in plugins_command()., Manifest reading edge cases., Test the install command., Test the update command., Reject path-traversal attempts while accepting valid names., Test the remove command. (+22 more)

### Community 62 - "provider_with_config() / TestToolHandlers"
Cohesion: 0.03
Nodes (26): _clean_env(), _make_mock_client(), provider(), provider_with_config(), Tests for the Hindsight memory provider plugin.  Tests cover config loading, too, When no config file exists, falls back to env vars., Ensure no stale env vars leak between tests., Helper to get the kwargs from the aretain_batch call. (+18 more)

### Community 63 - "_run() / memento_cards.py"
Cohesion: 0.05
Nodes (35): cmd_add(), cmd_add_quiz(), cmd_delete(), cmd_delete_collection(), cmd_due(), cmd_export(), cmd_import(), cmd_list() (+27 more)

### Community 64 - "anthropic_adapter.py / build_anthropic_client()"
Cohesion: 0.04
Nodes (75): build_anthropic_client(), build_anthropic_kwargs(), _common_betas_for_base_url(), _convert_content_part_to_anthropic(), _convert_content_to_anthropic(), convert_messages_to_anthropic(), _convert_openai_image_part_to_anthropic(), convert_tools_to_anthropic() (+67 more)

### Community 65 - "_make_sessions() / TestCursesBrowse"
Cohesion: 0.04
Nodes (39): _make_sessions(), Tests for the interactive session browser (`hermes sessions browse`).  Covers: -, Invalid selection followed by valid one works., KeyboardInterrupt in fallback mode returns None., Fallback mode should display all session entries., When a session has a title, show it instead of the preview., When no title, show preview., Generate a list of fake rich-session dicts. (+31 more)

### Community 66 - "TestValidateImageUrl / test_vision_tools.py"
Cohesion: 0.03
Nodes (22): Tests for tools/vision_tools.py — URL validation, type hints, error logging., Verify _handle_vision_analyze returns an Awaitable and builds correct prompt., The handler must return an Awaitable (coroutine) since it's registered as async., The full prompt should incorporate the user's question., AUXILIARY_VISION_MODEL env var should override DEFAULT_VISION_MODEL., Without AUXILIARY_VISION_MODEL, model should be None (let call_llm resolve defau, Missing keys should default to empty strings, not raise., Verify that exc_info=True is used in error/warning log calls. (+14 more)

### Community 67 - "rl_training_tool.py / _make_run_state()"
Cohesion: 0.04
Nodes (56): check_rl_api_keys(), check_rl_python_version(), _ensure_logs_dir(), EnvironmentInfo, _get_env_config_fields(), get_missing_keys(), _initialize_environments(), _monitor_training_run() (+48 more)

### Community 68 - "profiles.py / delete_profile()"
Cohesion: 0.05
Nodes (67): check_alias_collision(), _check_gateway_running(), _cleanup_gateway_service(), _count_skills(), create_profile(), create_wrapper_script(), _default_export_ignore(), delete_profile() (+59 more)

### Community 69 - "test_read_loop_detection. / TestTodoInjectionFilterin"
Cohesion: 0.03
Nodes (18): _fake_read_file(), _FakeReadResult, _FakeSearchResult, _make_fake_file_ops(), Verify that notify_other_tool_call resets the consecutive counter., Verify get_read_files_summary returns accurate file-read history., Verify clear_read_tracker resets state properly., Verify that search_tool detects and blocks consecutive repeated searches. (+10 more)

### Community 70 - "skills_tool.py / error_classifier.py"
Cohesion: 0.05
Nodes (63): Enum, _classify_400(), _classify_402(), classify_api_error(), _classify_by_error_code(), _classify_by_message(), _classify_by_status(), _extract_error_body() (+55 more)

### Community 71 - "approval.py / check_all_command_guards("
Cohesion: 0.04
Nodes (65): _approval_key_aliases(), _ApprovalEntry, approve_permanent(), approve_session(), check_all_command_guards(), check_dangerous_command(), clear_session(), detect_dangerous_command() (+57 more)

### Community 72 - "test_run_agent_codex_resp / _build_agent()"
Cohesion: 0.06
Nodes (58): _build_agent(), _build_copilot_agent(), _codex_ack_message_response(), _codex_commentary_message_response(), _codex_incomplete_message_response(), _codex_message_response(), _codex_reasoning_only_response(), _codex_request_kwargs() (+50 more)

### Community 73 - "_skill_dir() / test_skill_manager_tool.p"
Cohesion: 0.04
Nodes (14): Tests for tools/skill_manager_tool.py — skill creation, editing, and deletion., Patch both SKILLS_DIR and get_all_skills_dirs so _find_skill searches     only t, _skill_dir(), TestCreateSkill, TestDeleteSkill, TestEditSkill, TestPatchSkill, TestRemoveFile (+6 more)

### Community 74 - "_make_response() / test_llm_content_none_gua"
Cohesion: 0.04
Nodes (31): _make_response(), Tests for None guard on response.choices[0].message.content.strip().  OpenAI-com, tools/web_tools.py — synthesize_content() final_summary line, tools/vision_tools.py — analyze_image() analysis extraction, tools/skills_guard.py — _llm_audit_skill() llm_text extraction, tools/session_search_tool.py — _summarize_session() return line, Read the actual source files and verify the fix is applied.      These tests wil, Build a minimal OpenAI-compatible ChatCompletion response stub.      Extra keywo (+23 more)

### Community 75 - "test_matrix_mention.py / _make_adapter()"
Cohesion: 0.05
Nodes (47): _ensure_nio_mock(), _make_adapter(), _make_event(), _make_room(), Tests for Matrix require-mention gating and auto-thread features., Default (require_mention=true): messages without mention are ignored., Install a mock nio module when matrix-nio isn't available., Default: messages with mention are processed, mention stripped. (+39 more)

### Community 76 - "test_cron_script.py / TestScriptPathContainment"
Cohesion: 0.03
Nodes (28): cron_env(), Tests for cron job script injection feature.  Tests cover: - Script field in job, Scripts can output structured JSON for the LLM to parse., Test that script output is injected into the prompt., Test the cronjob tool's script parameter., Isolated cron environment with temp HERMES_HOME., Regression tests for path containment bypass in _run_job_script().      Prior to, Absolute paths outside ~/.hermes/scripts/ must be rejected. (+20 more)

### Community 77 - "TestCmdMigrate / test_claw.py"
Cohesion: 0.03
Nodes (22): Tests for hermes claw commands., Test directory archival (rename)., Test the claw_command router., Test script discovery in known locations., Test the migrate command handler., After successful migration, _offer_source_archival should be called., Dry run should not offer archival., The 'full' preset should set migrate_secrets=True automatically. (+14 more)

### Community 78 - "TestFilterAndSummarize / test_homeassistant_tool.p"
Cohesion: 0.03
Nodes (16): Tests for the Home Assistant tool module.  Tests real logic: entity filtering, p, Verify dangerous HA service domains are blocked., Safe domains like 'light' should not be blocked (will fail on network, not block, Verify entity_id format validation prevents path traversal., Some services (like scene.turn_on) don't need entity_id., Registry should exclude HA tools when HASS_TOKEN is not set., Registry should include HA tools when HASS_TOKEN is set., TestBuildServicePayload (+8 more)

### Community 79 - "blackbox / docker-management"
Cohesion: 0.03
Nodes (64): 3d, agentmail, agentmail, AI, animation, ascii-art, blackbox, Blackbox (+56 more)

### Community 80 - "display.py / _get_skin()"
Cohesion: 0.04
Nodes (61): build_tool_preview(), capture_local_edit_snapshot(), _detect_tool_failure(), _diff_from_snapshot(), _display_diff_path(), _emit_inline_diff(), extract_edit_diff(), format_context_pressure() (+53 more)

### Community 81 - "test_mattermost.py / TestMattermostFormatMessa"
Cohesion: 0.04
Nodes (16): _make_adapter(), test_audio_media_type_is_full_mime(), test_dm_always_responds(), test_document_media_type_is_full_mime(), test_free_response_channel_responds_without_mention(), test_image_media_type_is_full_mime(), test_mention_stripped_from_text(), test_non_free_channel_still_requires_mention() (+8 more)

### Community 82 - "TestSyncSkills / ._patches()"
Cohesion: 0.05
Nodes (26): Tests for tools/skills_sync.py — manifest-based skill seeding and updating., Create a fake bundled skills directory., Return context manager stack for patching sync globals., After fresh install, manifest should have v2 format with hashes., Skill in manifest but not on disk = user deleted it. Don't re-add., Skill in manifest + on disk + user hasn't modified = update from bundled., Skill modified by user should NOT be overwritten even if bundled changed., Skill in sync (user == bundled == origin) = no action needed. (+18 more)

### Community 83 - "wecom.py / ._send_media_source()"
Cohesion: 0.06
Nodes (22): _apply_file_size_limits(), check_wecom_requirements(), _coerce_list(), _decode_base64(), _decrypt_file_bytes(), _derive_message_type(), _detect_image_ext(), _detect_wecom_media_type() (+14 more)

### Community 84 - "SkinConfig / skin_engine.py"
Cohesion: 0.05
Nodes (44): _build_skin_config(), get_active_goodbye(), get_active_help_header(), get_active_prompt_symbol(), get_active_skin(), get_active_skin_name(), get_prompt_toolkit_style_overrides(), init_skin_from_config() (+36 more)

### Community 85 - "test_homeassistant.py / TestFormatStateChange"
Cohesion: 0.06
Nodes (27): fmt(), _make_adapter(), _make_event(), _mock_aiohttp_session(), test_cooldown_blocks_rapid_events(), test_cooldown_expires(), test_different_entities_independent_cooldowns(), test_empty_entity_id_skipped() (+19 more)

### Community 86 - "_extract() / TestBasicDetection"
Cohesion: 0.05
Nodes (22): _extract(), Tests for extract_local_files() — auto-detection of bare local file paths in mod, Paths that don't exist on disk are not extracted., Mix of existing and non-existing — only existing are returned., Paths embedded in HTTP URLs must not be extracted., ~/photos/a.png and /home/user/photos/a.png are the same file., Run extract_local_files with os.path.isfile mocked to return True     for any pa, The raw ~/... form should be removed, not the expanded /home/user/... form. (+14 more)

### Community 87 - "rate_limit_tracker.py / TestFormatting"
Cohesion: 0.05
Nodes (27): _bar(), _bucket_line(), _fmt_count(), _fmt_seconds(), format_rate_limit_compact(), format_rate_limit_display(), parse_rate_limit_headers(), RateLimitBucket (+19 more)

### Community 88 - "test_redact.py / TestEnvAssignments"
Cohesion: 0.03
Nodes (15): _ensure_redaction_enabled(), Tests for agent.redact -- secret masking in logs and output., Ensure HERMES_REDACT_SECRETS is not disabled by prior test imports., Simulate what happens when the agent runs `env` or `printenv`., Regression tests for ElevenLabs (sk_), Tavily (tvly-), and Exa (exa_) keys., TestAuthHeaders, TestElevenLabsTavilyExaKeys, TestEnvAssignments (+7 more)

### Community 89 - "model_metadata.py / get_model_context_length("
Cohesion: 0.06
Nodes (58): _add_model_aliases(), _coerce_reasonable_int(), detect_local_server_type(), estimate_messages_tokens_rough(), estimate_request_tokens_rough(), estimate_tokens_rough(), _extract_context_length(), _extract_first_int() (+50 more)

### Community 90 - "._make_resp() / TestQueryLocalContextLeng"
Cohesion: 0.05
Nodes (33): Tests for _query_local_context_length and the local server fallback in get_model, Reads max_model_len from /v1/models/{model} response., Reads context_length from /v1/models/{model} response., _query_local_context_length: falls back to /v1/models list., Finds context length for model in /v1/models list., Returns None when model is not in the /v1/models list., _query_local_context_length with LM Studio native /api/v1/models response., Build a mock httpx.Client with sequenced GET responses. (+25 more)

### Community 91 - "test_telegram_network.py / ._patch_doh()"
Cohesion: 0.07
Nodes (31): _doh_answer(), _fake_transport_factory(), FakeDoHClient, _make_response(), _telegram_request(), test_aclose_closes_all_transports(), test_all_doh_ips_same_as_system_dns_uses_seed(), test_all_ips_fail_raises_last_error() (+23 more)

### Community 92 - "test_ansi_strip.py / TestStripAnsiPassthrough"
Cohesion: 0.04
Nodes (26): Comprehensive tests for ANSI escape sequence stripping (ECMA-48).  The strip_ans, Device Control String sequences., 8-bit C1 control characters., Select Graphic Rendition — the most common ANSI sequences., Real-world contamination scenarios from bug reports., The original reported bug: shebang corrupted by color codes., Clean content must pass through unmodified., Array indexing must not be confused with CSI. (+18 more)

### Community 93 - "TestGeminiModelsDev / test_gemini_provider.py"
Cohesion: 0.04
Nodes (13): Tests for Google AI Studio (Gemini) provider integration., Verify run_agent.py has no SyntaxError (the critical bug)., Gemini falls through to chat_completions — no special elif needed., list_agentic_models filters correctly from mock models.dev data., TestGeminiAgentInit, TestGeminiAliases, TestGeminiAutoDetection, TestGeminiContextLength (+5 more)

### Community 94 - "TestSetupLogging / hermes_logging.py"
Cohesion: 0.04
Nodes (26): _add_rotating_handler(), _ManagedRotatingFileHandler, Enable DEBUG-level console logging for ``--verbose`` / ``-v`` mode.      Called, RotatingFileHandler that ensures group-writable perms in managed mode.      In m, Add a ``RotatingFileHandler`` to *logger*, skipping if one already     exists fo, Best-effort read of ``logging.*`` from config.yaml.      Returns ``(level, max_s, Configure the Hermes logging subsystem.      Safe to call multiple times — the s, _read_logging_config() (+18 more)

### Community 95 - "test_discord_slash_comman / discord.py"
Cohesion: 0.06
Nodes (26): allow_always(), allow_once(), allow_session(), check_discord_requirements(), deny(), _load_participated_threads(), ModelPickerView, no_btn() (+18 more)

### Community 96 - "test_update_gateway_resta / _make_run_side_effect()"
Cohesion: 0.04
Nodes (32): _make_run_side_effect(), Tests for cmd_update gateway auto-restart — systemd + launchd coverage.  Ensures, The generated launchd plist must include --replace so respawned     gateways kil, --replace comes after 'run' in the ProgramArguments., refresh_launchd_plist_if_needed rewrites stale plists (like systemd's     refres, launchd_start refreshes the plist before starting., launchd_start self-heals when the plist file is missing entirely., cmd_update correctly detects and handles launchd on macOS. (+24 more)

### Community 97 - "test_api_server_jobs.py / _create_app()"
Cohesion: 0.06
Nodes (52): adapter(), auth_adapter(), _create_app(), _make_adapter(), Tests for the Cron Jobs API endpoints on the API server adapter.  Covers: - CRUD, Create an adapter with optional API key., Create the aiohttp app with jobs routes registered., test_auth_passes_with_valid_key() (+44 more)

### Community 98 - "browser_camofox.py / _get_session()"
Cohesion: 0.07
Nodes (51): camofox_back(), camofox_click(), camofox_close(), camofox_console(), camofox_get_images(), camofox_navigate(), camofox_press(), camofox_scroll() (+43 more)

### Community 99 - "TestClarifySchema / TestClarifyToolBasics"
Cohesion: 0.04
Nodes (31): Tests for tools/clarify_tool.py - Interactive clarifying questions., Non-list choices should return error., Non-string choices should be converted to strings., Tests for callback error handling., Should return error if callback raises exception., Callback should receive trimmed question., User response should be stripped of whitespace., Tests for the requirements check function. (+23 more)

### Community 100 - "_make_cli() / TestDisplayResumedHistory"
Cohesion: 0.08
Nodes (24): _large_history(), _make_cli(), _multimodal_history(), Tests for session resume history display — _display_resumed_history() and _prelo, Conversation with multimodal (image) content., _display_resumed_history() renders a Rich panel with conversation recap., Run _display_resumed_history and capture the Rich console output., Create a HermesCLI instance with minimal mocking. (+16 more)

### Community 101 - "TestScanCronPrompt / TestScheduleCronjob"
Cohesion: 0.04
Nodes (9): Tests for tools/cronjob_tools.py — prompt scanning, schedule/list/remove dispatc, Cron is internal (JSON-based scheduler), no system crontab needed., Without any session env vars, cronjob tool should not be available., TestCronjobRequirements, TestListCronjobs, TestRemoveCronjob, TestScanCronPrompt, TestScheduleCronjob (+1 more)

### Community 102 - "test_logs.py / TestMatchesFilters"
Cohesion: 0.04
Nodes (14): log_dir(), Tests for hermes_cli/logs.py — log viewing and filtering., Create a fake HERMES_HOME with a logs/ directory., Write a realistic agent.log with mixed levels and sessions., Write a small errors.log., sample_agent_log(), sample_errors_log(), TestExtractLevel (+6 more)

### Community 103 - "test_supermemory_provider / FakeClient"
Cohesion: 0.04
Nodes (23): FakeClient, container_tag with {identity} resolves to profile-scoped tag., Without agent_identity kwarg, {identity} resolves to 'default'., SUPERMEMORY_CONTAINER_TAG env var overrides config., search_mode from config is passed to _SupermemoryClient., Invalid search_mode falls back to 'hybrid'., Multi-container is off by default; schemas have no container_tag param., When enabled, tool schemas include container_tag parameter. (+15 more)

### Community 104 - "_make_cli() / test_cli_init.py"
Cohesion: 0.06
Nodes (23): _make_cli(), Tests for HermesCLI initialization -- catches configuration bugs that only manif, When agent is running, /queue should still put the prompt in _pending_input., Create a HermesCLI instance with minimal mocking., When agent is idle, /queue should still queue (not reject)., In queue mode, Enter while busy should go to _pending_input, not _interrupt_queu, In interrupt mode (default), Enter while busy goes to _interrupt_queue., Single-query mode calls chat() without going through run(). (+15 more)

### Community 105 - "base_client.py / cmd_contract()"
Cohesion: 0.08
Nodes (47): cmd_contract(), cmd_gas(), cmd_price(), cmd_stats(), cmd_token(), cmd_tx(), cmd_wallet(), cmd_whales() (+39 more)

### Community 106 - "test_signal.py / _make_signal_adapter()"
Cohesion: 0.08
Nodes (27): _make_signal_adapter(), _stub_rpc(), test_fetch_attachment_handles_dict_response(), test_fetch_attachment_returns_none_on_empty(), test_fetch_attachment_uses_id_parameter(), test_send_document_error_includes_path(), test_send_document_too_large(), test_send_image_file_missing() (+19 more)

### Community 107 - "test_file_read_guards.py / _make_fake_ops()"
Cohesion: 0.05
Nodes (29): _FakeReadResult, _make_fake_ops(), Re-reading an unchanged file should return a lightweight stub., reset_file_dedup should clear the dedup cache so post-compression     reads retu, Large truncated files should include a hint about targeted reads., Minimal stand-in for FileOperations.read_file return value., file_read_max_chars in config.yaml should control the char guard., Paths like /dev/zero should be rejected before any I/O. (+21 more)

### Community 108 - "TestGetSectionConfigSumma / TestOfferOpenclawMigratio"
Cohesion: 0.05
Nodes (23): _first_time_args(), Tests for OpenClaw migration integration in the setup wizard., Should return False when user sees preview but declines to proceed., Test the _offer_openclaw_migration helper in isolation., Should catch exceptions and return False., Should return False immediately when ~/.openclaw does not exist., Should bootstrap config.yaml before running migration., Verify _offer_openclaw_migration is called during first-time setup. (+15 more)

### Community 109 - "tts_tool.py / text_to_speech_tool()"
Cohesion: 0.07
Nodes (44): _check_neutts_available(), check_tts_requirements(), _convert_to_opus(), _default_neutts_ref_audio(), _default_neutts_ref_text(), _generate_edge_tts(), _generate_elevenlabs(), _generate_minimax_tts() (+36 more)

### Community 110 - "._load_json() / pairing.py"
Cohesion: 0.07
Nodes (27): _cmd_approve(), _cmd_clear_pending(), _cmd_list(), _cmd_revoke(), pairing_command(), DM Pairing System  Code-based approval flow for authorizing new users on messagi, Check if a user is approved (paired) on a platform., List approved users, optionally filtered by platform. (+19 more)

### Community 111 - "status.py / acquire_scoped_lock()"
Cohesion: 0.08
Nodes (45): acquire_scoped_lock(), _build_pid_record(), _build_runtime_status_record(), check_mark(), _configured_model_label(), _effective_provider_label(), _format_iso_timestamp(), _get_lock_dir() (+37 more)

### Community 112 - "_install_telegram_mock() / test_send_message_tool.py"
Cohesion: 0.07
Nodes (17): _ensure_slack_mock(), _install_telegram_mock(), _make_config(), Tests for tools/send_message_tool.py., Messages exceeding the platform limit are split into multiple sends., Bold+italic ***text*** survives tool-layer formatting., Blockquote '>' markers must survive formatting (not escaped to '&gt;')., Pre-escaped HTML entities survive tool-layer formatting without double-escaping. (+9 more)

### Community 113 - "_make_agent() / TestTryRecoverPrimaryTran"
Cohesion: 0.08
Nodes (20): _make_agent(), _make_tool_defs(), _make_transport_error(), _mock_resolve(), Tests for per-turn primary runtime restoration and transport recovery.  Verifies, After restore, the full fallback chain should be available again., If client rebuild fails, the method returns False gracefully., Create an exception whose type().__name__ matches the given name. (+12 more)

### Community 114 - "TestToolKindMap / TestBuildToolTitle"
Cohesion: 0.04
Nodes (16): Tests for acp_adapter.tools — tool kind mapping and ACP content building., patch should produce a FileEditToolCallContent (diff)., write_file should produce a FileEditToolCallContent (diff)., terminal should produce text content with the command., read_file should include the path in content., search_files should include pattern in content., Unknown tools should get a generic text representation., Completed terminal call should include output text. (+8 more)

### Community 115 - "test_docker_environment.p / _make_dummy_env()"
Cohesion: 0.06
Nodes (42): _FakePopen, _make_dummy_env(), _make_execute_only_env(), _mock_subprocess_run(), Opt-in docker cwd mounting should bind the host cwd to /workspace., Mock subprocess.run to intercept docker run -d and docker version calls.      Re, Host cwd should not be mounted unless the caller explicitly opts in., Explicit user volumes for /workspace should take precedence over cwd mount. (+34 more)

### Community 116 - "_make_skill() / TestScanSkillCommands"
Cohesion: 0.06
Nodes (18): _make_skill(), Tests for agent/skill_commands.py — skill slash command scanning and platform fi, Skill names with +, /, or other special chars produce clean cmd keys., Skill with name consisting only of special chars is silently skipped., Skill names with / chars produce clean cmd keys., Telegram bot-command names disallow hyphens, so the menu registers     skills wi, /claude_code from Telegram autocomplete must resolve to /claude-code., A user-typed /foo-bar (hyphen) must not trigger the underscore fallback. (+10 more)

### Community 117 - "commands.py / .get_completions()"
Cohesion: 0.07
Nodes (40): _build_command_lookup(), _build_description(), _clamp_command_names(), _collect_gateway_skill_entries(), _completion_text(), _context_completions(), discord_skill_commands(), _extract_context_word() (+32 more)

### Community 118 - "TestDogfoodSkill / test_browser_console.py"
Cohesion: 0.05
Nodes (17): Tests for browser_console tool and browser_vision annotate param., browser_console is properly registered in the tool registry., browser_console must be reachable via toolset resolution., browser_vision supports annotate parameter., Without annotate, screenshot command has no --annotate flag., browser_console() returns console messages + JS errors in one call., With annotate=True, screenshot command includes --annotate., browser.record_sessions config option. (+9 more)

### Community 119 - "test_mcp_config.py / _make_args()"
Cohesion: 0.07
Nodes (20): FakeTool, _isolate_config(), _make_args(), Tests for hermes_cli.mcp_config — ``hermes mcp`` subcommands.  These tests mock, Server without explicit enabled key defaults to enabled., Must specify --url or --command., Add an HTTP server, accept all tools., Redirect all config I/O to a temp directory. (+12 more)

### Community 120 - "test_website_policy.py / website_policy.py"
Cohesion: 0.06
Nodes (21): Missing shared blocklist files are warned and skipped, not fatal., Malformed config with default path should fail open (return None), not crash., test_browser_navigate_allows_when_shared_file_missing(), test_check_website_access_fails_open_on_malformed_config(), check_website_access(), _extract_host_from_urlish(), _get_default_config_path(), invalidate_cache() (+13 more)

### Community 121 - "test_update_autostash.py / _setup_update_mocks()"
Cohesion: 0.07
Nodes (32): _make_update_side_effect(), When conflicts occur interactively, user is prompted before reset., When user declines reset, working tree is left as-is., Non-interactive mode auto-resets without prompting and returns False     instead, Common setup for cmd_update tests., When .[all] fails, update should keep base deps and retry extras individually., When .[all] succeeds, no fallback should be attempted., Build a subprocess.run side_effect for cmd_update tests. (+24 more)

### Community 122 - "FakeHAServer / test_ha_integration.py"
Cohesion: 0.07
Nodes (19): FakeHAServer, Fake Home Assistant server for integration testing.  Provides a real HTTP + WebS, Enqueue a state_changed event for delivery over WebSocket., Return a 401 response if the Bearer token is wrong, else None., In-process fake Home Assistant for integration tests.      Parameters     ------, _adapter_for(), Integration tests for Home Assistant (tool + gateway).  Spins up a real in-proce, Call the async tool functions directly against the fake server.      Note: we ca (+11 more)

### Community 123 - "test_skills_config.py / TestGetDisabledSkillNames"
Cohesion: 0.05
Nodes (13): Tests for hermes_cli/skills_config.py and skills_tool disabled filtering., Tests for agent.skill_utils.get_disabled_skill_names., Explicit platform= parameter should resolve per-platform list., HERMES_SESSION_PLATFORM should be used when HERMES_PLATFORM is unset., HERMES_PLATFORM should win over HERMES_SESSION_PLATFORM., Explicit platform= param should override all env vars., No platform env vars or param should return global list., TestFindAllSkillsFiltering (+5 more)

### Community 124 - "test_pairing.py / TestApprovalFlow"
Cohesion: 0.05
Nodes (13): _make_store(), Tests for gateway/pairing.py — DM pairing security system., Create a PairingStore with PAIRING_DIR pointed to tmp_path., Multiple codes for different users should be distinct., TestApprovalFlow, TestCodeExpiry, TestCodeGeneration, TestListAndClear (+5 more)

### Community 125 - "test_browser_homebrew_pat / TestDiscoverHomebrewNodeD"
Cohesion: 0.05
Nodes (23): Tests for macOS Homebrew PATH discovery in browser_tool.py., Should find npx in Homebrew paths as a fallback., Should raise FileNotFoundError when nothing works., Verify _run_browser_command() includes Homebrew node dirs in subprocess PATH., A local agent-browser path containing spaces must stay one argv entry., Verify _SANE_PATH includes Homebrew directories., The synthetic npx fallback should still expand into separate argv items., When _discover_homebrew_node_dirs returns dirs, they should appear         in th (+15 more)

### Community 126 - "test_command_guards.py / TestContainerSkip"
Cohesion: 0.05
Nodes (16): _clean_state(), Tests for check_all_command_guards() — combined tirith + dangerous command guard, When tools.tirith_security can't be imported, treated as allow., Clear approval state and relevant env vars between tests., Tirith 'block' is now treated as an approvable warning (not a hard block)., TestAlwaysVisibility, TestCombinedWarnings, TestContainerSkip (+8 more)

### Community 127 - "TestIsSafeUrl / test_url_safety.py"
Cohesion: 0.05
Nodes (14): Tests for SSRF protection in url_safety module., ::ffff:127.0.0.1 — IPv4-mapped IPv6 loopback., ::ffff:169.254.169.254 — IPv4-mapped IPv6 cloud metadata., 0.0.0.0 — unspecified address, can bind to all interfaces., Unexpected exceptions should block, not allow., fc00::/7 — IPv6 unique local addresses., 100.0.0.1 is NOT in CGNAT range (100.64.0.0/10), should be allowed., Direct tests for the _is_blocked_ip helper. (+6 more)

### Community 128 - "TestResolveToken / TestTokenValidation"
Cohesion: 0.05
Nodes (14): Tests for hermes_cli.copilot_auth — Copilot token validation and resolution., Copilot API header generation., The models.py copilot_default_headers uses copilot_auth., API mode selection matching opencode's shouldUseCopilotResponsesApi., PROVIDER_REGISTRY has correct env var order., Token resolution with env var priority., Classic PATs in env vars should be skipped, not returned., Token type validation. (+6 more)

### Community 129 - "test_telegram_documents.p / _make_message()"
Cohesion: 0.12
Nodes (24): _ensure_telegram_mock(), _make_document(), _make_file_obj(), _make_message(), _make_photo(), _make_update(), _redirect_cache(), test_caption_preserved_with_injection() (+16 more)

### Community 130 - "_run_auxiliary_bridge() / TestAuxiliaryConfigBridge"
Cohesion: 0.06
Nodes (18): Tests for auxiliary model config bridging — verifies that config.yaml values are, Config without auxiliary section should not crash., Malformed task config (e.g. string instead of dict) is safely ignored., Verify the gateway/run.py config bridge contains the auxiliary section., Simulate the auxiliary config → env var bridging logic shared by CLI and gateway, The gateway config bridge must include auxiliary.* bridging., Gateway should NOT bridge compression config to env vars (config-only)., Test that AUXILIARY_VISION_MODEL env var overrides the default model in the hand (+10 more)

### Community 131 - "make_tc() / TestCapDelegateTaskCalls"
Cohesion: 0.08
Nodes (10): assistant_dict_call(), make_tc(), Unit tests for AIAgent pre/post-LLM-call guardrails.  Covers three static method, Create a minimal tool_call SimpleNamespace mirroring the OpenAI SDK object., Dict-style tool_call (as stored in message history)., TestCapDelegateTaskCalls, TestDeduplicateToolCalls, TestGetToolCallIdStatic (+2 more)

### Community 132 - "clipboard.py / has_clipboard_image()"
Cohesion: 0.08
Nodes (38): _convert_to_png(), _find_powershell(), _get_ps_exe(), has_clipboard_image(), _is_wsl(), _linux_save(), _macos_has_image(), _macos_osascript() (+30 more)

### Community 133 - "TestHermesParser / TestMistralParser"
Cohesion: 0.05
Nodes (10): Tests for environments/tool_call_parsers/ — client-side tool call parsers.  Thes, Test handling of unclosed tool_call tag (model truncated mid-generation)., Ensure all parsers conform to the ParseResult contract., When tool calls are found, they should be ChatCompletionMessageToolCall objects., Every registered parser should be importable and instantiable., TestDeepSeekV3Parser, TestHermesParser, TestMistralParser (+2 more)

### Community 134 - "_make_agent() / TestTryActivateFallback"
Cohesion: 0.1
Nodes (16): _make_agent(), _make_tool_defs(), _mock_resolve(), Tests for the provider fallback model feature.  Verifies that AIAgent can switch, Fallback should fail gracefully when the API key env var is unset., Custom base_url in config should override the provider default., Z.AI should also check Z_AI_API_KEY as fallback env var., OpenAI Codex fallback should use OAuth credentials and codex_responses mode. (+8 more)

### Community 135 - "test_openclaw_migration.p / load_module()"
Cohesion: 0.09
Nodes (38): load_module(), load_skills_guard(), Discord bot token and allowlist migrate to .env., Slack bot/app tokens and allowlist migrate to .env., Signal account, HTTP URL, and allowlist migrate to .env., Default model setting migrates to config.yaml., Model config handles {primary: ...} object format., TTS provider and voice settings migrate to config.yaml. (+30 more)

### Community 136 - "TestSessionSearch / test_session_search.py"
Cohesion: 0.05
Nodes (12): Tests for tools/session_search_tool.py — helper functions and search dispatcher., session_search should never return the current session., Other sessions should still be returned when current is excluded., Verify the _HIDDEN_SESSION_SOURCES constant used for third-party isolation., Compression/delegation parents should be excluded for the active child session., Delegation child hits should be excluded when they resolve to the current root s, TestFormatConversation, TestFormatTimestamp (+4 more)

### Community 137 - "test_file_tools.py / TestFileToolsList"
Cohesion: 0.05
Nodes (12): Tests for the file tools module (schema, handler wiring, error paths).  Tests ve, Patch tool should hint when old_string is not found., Search tool should hint when results are truncated., Clear read/search tracker between tests to avoid cross-test state., All schemas must have name, description, and parameters with properties., TestFileToolsList, TestPatchHandler, TestPatchHints (+4 more)

### Community 138 - "test_osv_check.py / TestCheckPackageForMalwar"
Cohesion: 0.05
Nodes (13): Tests for OSV malware check on MCP extension packages., Known malware package returns error string., Network errors allow the package (fail-open)., Non-npx/uvx commands are skipped entirely., uvx commands check PyPI ecosystem., Live integration test against the real OSV API. Skipped if offline., Clean package returns None (allow)., TestCheckPackageForMalware (+5 more)

### Community 139 - "test_auth_qwen_provider.p / _make_qwen_tokens()"
Cohesion: 0.09
Nodes (26): _make_qwen_tokens(), qwen_env(), Tests for Qwen OAuth provider authentication (hermes_cli/auth.py).  Covers: _qwe, When expires_in is missing, default to 6 hours., Create a minimal Qwen CLI OAuth credential dict., Write tokens to the Qwen CLI credentials file and return the path., Redirect _qwen_cli_auth_path to tmp_path/.qwen/oauth_creds.json., test_get_qwen_auth_status_logged_in() (+18 more)

### Community 140 - "TestExtractPathWord / _display_names()"
Cohesion: 0.07
Nodes (10): _display_metas(), _display_names(), Tests for file path autocomplete in the CLI completer., Test the completer produces path completions via the prompt_toolkit API., Extract plain-text display names from a list of Completion objects., Extract plain-text display_meta from a list of Completion objects., TestExtractPathWord, TestFileSizeLabel (+2 more)

### Community 141 - "_StubAdapter / test_send_retry.py"
Cohesion: 0.07
Nodes (14): _StubAdapter, test_connect_timeout_still_retried(), test_fallback_failure_logged_but_not_raised(), test_network_to_nonnetwork_transition_falls_back_to_plaintext(), test_non_network_error_falls_back_immediately(), test_notice_send_exception_doesnt_propagate(), test_retries_on_connect_error_and_succeeds(), test_retryable_flag_respected() (+6 more)

### Community 142 - "test_model_tools_async_br / TestRunAsyncWorkerThread"
Cohesion: 0.07
Nodes (26): _create_and_return_transport(), _get_current_loop(), _mock_vision_response(), Regression tests for the _run_async() event-loop lifecycle.  These tests verify, Multiple _run_async calls on the same worker thread should         reuse the sam, Different worker threads must get their own loops to avoid         contention (t, Worker thread loops must be different from the main thread's         persistent, When a loop is already running, _run_async falls back to a thread. (+18 more)

### Community 143 - "_enable_persistence() / test_browser_camofox_pers"
Cohesion: 0.08
Nodes (14): _enable_persistence(), _mock_response(), Persistence tests for the Camofox browser backend.  Tests that managed persisten, With managed_persistence: stable userId derived from Hermes profile., VNC URL is derived from the Camofox health endpoint., camofox_soft_cleanup drops local state only when managed persistence is on., Soft cleanup must never hit the Camofox /sessions DELETE endpoint., Return a patch context that enables managed persistence via config. (+6 more)

### Community 144 - "TestCoalesceSessionNameAr / test_coalesce_session_arg"
Cohesion: 0.05
Nodes (19): Tests for _coalesce_session_name_args — multi-word session name merging., hermes -c my project sessions list → stops before 'sessions, hermes -c my setup → 'setup' is a subcommand, not part of name, hermes -c Pokemon Agent Dev → -c 'Pokemon Agent Dev, hermes --continue Pokemon Agent Dev, hermes -c MyProject (no merging needed), hermes -c 'Pokemon Agent Dev' (shell already merged), hermes -c (no name — means 'continue latest') (+11 more)

### Community 145 - "TestBuildToolPreview / TestEditDiffPreview"
Cohesion: 0.05
Nodes (12): Tests for agent/display.py — build_tool_preview() and inline diff previews., Tests for build_tool_preview defensive handling and normal operation., PR #453: None args should not crash, should return None., Empty dict has no keys to preview., Known tool with its primary arg should return a preview string., Unknown tool but with a recognized fallback key should still preview., Unknown tool with no recognized keys should return None., Preview should truncate long values. (+4 more)

### Community 146 - "TestMinimaxBetaHeaders / ._build_and_get_betas()"
Cohesion: 0.06
Nodes (12): Tests for MiniMax provider hardening — context lengths, thinking guard, catalog,, MiniMax Anthropic-compat endpoints reject fine-grained-tool-streaming beta., Build client, return the anthropic-beta header string., Verify that build_anthropic_kwargs does NOT add thinking params for MiniMax mode, Verify per-model context length entries for MiniMax models., Verify auxiliary model is standard (not highspeed)., Verify the model catalog includes M1 family and excludes deprecated models., TestMinimaxAuxModel (+4 more)

### Community 147 - "test_whatsapp_connect.py / _make_adapter()"
Cohesion: 0.09
Nodes (25): _AsyncCM, _bare_adapter(), _connect_patches(), _make_adapter(), _mock_aiohttp(), Tests for WhatsApp connect() error handling.  Regression tests for two bugs in W, Direct tests for the _close_bridge_log() helper method., Minimal async context manager returning a fixed value. (+17 more)

### Community 148 - "solana_client.py / print_json()"
Cohesion: 0.1
Nodes (34): cmd_activity(), cmd_nft(), cmd_price(), cmd_stats(), cmd_token(), cmd_tx(), cmd_wallet(), cmd_whales() (+26 more)

### Community 149 - "test_tools_config.py / TestPlatformToolsetConsis"
Cohesion: 0.06
Nodes (22): Tests for hermes_cli.tools_config platform tool persistence., Ensure MCP server names are preserved when saving platform tools.      Regressio, Saving platform tools works when no existing config exists., Saving platform tools works when existing config is not a list., Platform default toolsets (hermes-cli, hermes-telegram, etc.) must NOT     be pr, Same bug for Telegram — hermes-telegram must not be preserved., MCP server names must still be preserved even when platform defaults     are bei, Every platform in tools_config.PLATFORMS must have a matching toolset. (+14 more)

### Community 150 - "FakeClientV2 / TestMem0FiltersV2"
Cohesion: 0.09
Nodes (14): FakeClientV2, Tests for Mem0 API v2 compatibility — filters param and dict response unwrapping, Read filters should use user_id only — cross-session recall across agents., Write filters should include agent_id for attribution., API v2 returns {"results": [...]} dicts; we must extract the list., Fake Mem0 client that returns v2-style dict responses and captures call kwargs., Old API returned bare lists — still works., Old API returned bare lists — still works. (+6 more)

### Community 151 - "test_cli_file_drop.py / TestNonFileInputs"
Cohesion: 0.06
Nodes (15): Tests for _detect_file_drop — file path detection that prevents dragged/pasted a, r"""macOS drags produce paths like /path/to/my\ file.png, A file literally named 'help' inside a directory starting with /., Create a temporary .png file and return its path., Create a temporary .py file and return its path., Create a file whose name contains spaces (like macOS screenshots)., A directory path should not be treated as a file drop., TestEdgeCases (+7 more)

### Community 152 - "test_events.py / TestStepCallback"
Cohesion: 0.06
Nodes (22): event_loop_fixture(), mock_conn(), Tests for acp_adapter.events — callback factories for ACP notifications., Thinking callback should emit AgentThoughtChunk., Empty text should not emit any update., Step callback should mark tracked tools as completed., Tools not in tool_call_ids should be silently ignored., Tool info as a string (just the name) should work. (+14 more)

### Community 153 - "test_wecom.py / TestMediaHelpers"
Cohesion: 0.06
Nodes (5): TestExtractText, TestMediaHelpers, TestPolicyHelpers, TestWeComAdapterInit, TestWeComRequirements

### Community 154 - "FakeAgent / TestInactivityTimeout"
Cohesion: 0.07
Nodes (19): FakeAgent, Tests for cron job inactivity-based timeout.  Tests cover: - Active agent runs i, An agent that goes idle should be detected and interrupted., HERMES_CRON_TIMEOUT=0 means no timeout at all., HERMES_CRON_TIMEOUT env var is respected., HERMES_CRON_TIMEOUT=0 yields None (unlimited)., The TimeoutError message should include last activity info., If agent lacks get_activity_summary, idle_secs stays 0 (never times out). (+11 more)

### Community 155 - "_make_skill_content() / test_skill_size_limits.py"
Cohesion: 0.07
Nodes (20): isolate_skills(), _make_skill_content(), Tests for skill content size limits.  Agent writes (create/edit/patch/write_file, patch action checks resulting size, not just the new_string., Patches that shrink an already-oversized skill should succeed., Patch on a supporting file also checks size., write_file action enforces both char and byte limits., Skills dropped directly on disk are not constrained. (+12 more)

### Community 156 - "_new_filter_matches() / TestNewFilterCrossPlatfor"
Cohesion: 0.07
Nodes (22): _new_filter_matches(), _old_filter_matches(), Tests for the hidden directory filter in skills listing.  Regression test: the o, The BROKEN filter that used hardcoded forward slashes.      Returns True when th, The FIXED filter using Path.parts.      Returns True when the path SHOULD be fil, Demonstrate the bug: hardcoded '/' never matches Windows backslash paths., Old filter fails to catch .hub in a Windows-style path string., Old filter fails to catch .git in a Windows-style path string. (+14 more)

### Community 157 - "_make_aiohttp_resp() / _make_aiohttp_session()"
Cohesion: 0.11
Nodes (12): _make_aiohttp_resp(), _make_aiohttp_session(), Tests for _send_mattermost, _send_matrix, _send_homeassistant, _send_dingtalk., Each call should generate a distinct transaction ID in the URL., Build a minimal async-context-manager mock for an aiohttp response., DingTalk always returns HTTP 200 but signals errors via errcode., If raise_for_status throws, the error is caught and returned., Wrap a response mock in a session mock that supports async-with for post/put. (+4 more)

### Community 158 - "test_set_config_value.py / _read_config()"
Cohesion: 0.09
Nodes (22): _isolated_hermes_home(), Tests for set_config_value — verifying secrets route to .env and config to confi, Regular config keys should go to config.yaml, NOT .env., TERMINAL_DOCKER_IMAGE doesn't match _API_KEY or _TOKEN, so config.yaml., config set should accept empty strings and falsy values like '0'., Blanking an API key should write an empty value to .env., Blanking a config key should write an empty string to config.yaml., Point HERMES_HOME at a temp dir so tests never touch real config. (+14 more)

### Community 159 - "TestHandleSkillsSlashInst / TestHandleSkillsSlashUnin"
Cohesion: 0.06
Nodes (18): Tests for skip_confirm and invalidate_cache behavior in /skills install and /ski, Without --now, cache invalidation is deferred to next session., --now opts into immediate cache invalidation., Test that do_install respects skip_confirm parameter., Test that do_uninstall respects skip_confirm parameter., With skip_confirm=True, input() should not be called., Without skip_confirm, input() should be called., Without skip_confirm, answering 'n' should cancel. (+10 more)

### Community 160 - "_make_cli() / TestCLIStatusBar"
Cohesion: 0.11
Nodes (11): _attach_agent(), _make_cli(), Ensure status bar fragments don't overflow the terminal width., Total fragment text length must not exceed the width used to build them., When prompt_toolkit reports a width, shutil.get_terminal_size must not be used., Outside a TUI context (no running app), shutil must be used as fallback., _build_status_bar_text() must also prefer prompt_toolkit width., An explicit width= argument must bypass both PT and shutil lookups. (+3 more)

### Community 161 - "generate_meme.py / _add_bars()"
Cohesion: 0.1
Nodes (32): _add_bars(), _default_fields(), draw_outlined_text(), fetch_imgflip_templates(), _fetch_url(), find_font(), generate_from_image(), generate_meme() (+24 more)

### Community 162 - "test_browser_camofox.py / _mock_response()"
Cohesion: 0.08
Nodes (24): _mock_response(), Tests for the Camofox browser backend., Verify that browser_tool.py delegates to camofox when CAMOFOX_URL is set., test_back(), test_browser_navigate_routes_to_camofox(), test_cleanup_all(), test_click(), test_close_session() (+16 more)

### Community 163 - "test_web_tools_tavily.py / TestNormalizeTavilyDocume"
Cohesion: 0.06
Nodes (17): Tests for Tavily web backend integration.  Coverage:   _tavily_request() — API k, Test extract/crawl document normalization., Test web_search_tool dispatch to Tavily., Test web_extract_tool dispatch to Tavily., Test suite for the _tavily_request helper., Test web_crawl_tool dispatch to Tavily., No TAVILY_API_KEY → ValueError with guidance., Instructions are included in the Tavily crawl payload. (+9 more)

### Community 164 - "SlowFakeAgent / TestStagedInactivityWarni"
Cohesion: 0.08
Nodes (17): FakeAgent, Tests for staged inactivity timeout in gateway agent runs.  Tests cover: - Warni, No warning fires when gateway_timeout_warning is 0., Warning fires exactly once even if agent remains idle., Full timeout fires even after warning was sent., HERMES_AGENT_TIMEOUT_WARNING env var is parsed correctly., HERMES_AGENT_TIMEOUT_WARNING=0 disables the warning., Mock agent with controllable activity summary for timeout tests. (+9 more)

### Community 165 - "Popular Web Designs Templ / Design System: Framer"
Cohesion: 0.06
Nodes (33): Popular Web Designs Template Collection, Framer Color System, Framer Components, Framer Typography Rules, Intercom Color System, Intercom Components, Intercom Typography Rules, Kraken Color System (+25 more)

### Community 166 - "homeassistant_tool.py / _async_call_service()"
Cohesion: 0.1
Nodes (31): _async_call_service(), _async_get_state(), _async_list_entities(), _async_list_services(), _build_service_payload(), _check_ha_available(), _filter_and_summarize(), _get_config() (+23 more)

### Community 167 - "TestResolveChannelName / ._setup()"
Cohesion: 0.1
Nodes (9): Tests for gateway/channel_directory.py — channel resolution and display., Write sessions.json at the path _build_from_sessions expects., Helper to write a fake channel directory., TestBuildChannelDirectoryWrites, TestBuildFromSessions, TestFormatDirectoryForDisplay, TestLoadDirectory, TestResolveChannelName (+1 more)

### Community 168 - "TestGetProvider / test_transcription.py"
Cohesion: 0.06
Nodes (9): Tests for transcription_tools.py — local (faster-whisper) and OpenAI providers., _get_provider() picks the right backend based on config + availability., Explicit local provider must not silently fall back to cloud., Explicit openai without key returns none — no cross-provider fallback., TestGetProvider, TestTranscribeAudio, TestTranscribeLocal, TestTranscribeOpenAI (+1 more)

### Community 169 - "WebToolsTester / .run_all_tests()"
Cohesion: 0.12
Nodes (21): Colors, main(), print_error(), print_header(), print_info(), print_section(), print_success(), print_warning() (+13 more)

### Community 170 - "test_dm_topics.py / _make_adapter()"
Cohesion: 0.14
Nodes (29): _make_adapter(), _make_mock_message(), test_build_message_event_no_auto_skill_without_binding(), test_build_message_event_no_auto_skill_without_thread(), test_build_message_event_sets_auto_skill(), test_cache_dm_topic_from_message(), test_cache_dm_topic_from_message_no_overwrite(), test_create_dm_topic_handles_duplicate_error() (+21 more)

### Community 171 - "Ascii-Video/References/Sh / Ascii-Video/References/Co"
Cohesion: 0.09
Nodes (31): Architecture, 20 Blend Modes, Animated Sine Field (General Purpose), ASCII Video Production Pipeline, Available Modes, Background Fills, Blend Mode Selection Guide, Composition & Brightness Reference (+23 more)

### Community 172 - "test_file_staleness.py / _make_fake_ops()"
Cohesion: 0.09
Nodes (14): _FakePatchResult, _FakeReadResult, _FakeWriteResult, _make_fake_ops(), test_different_task_isolated(), test_no_warning_for_new_file(), test_no_warning_when_file_never_read(), test_no_warning_when_file_unchanged() (+6 more)

### Community 173 - "_build_parser() / test_argparse_flag_propag"
Cohesion: 0.11
Nodes (12): _build_parser(), Tests for parent→subparser flag propagation.  When flags like --yolo, -w, -s exi, When no subcommand is given, flags must work and defaults must hold., Verify --yolo sets HERMES_YOLO_MODE regardless of flag position.      This tests, Replicate the exact check from cmd_chat in main.py., Build the hermes argument parser from the real code.      We import the real mai, Flags placed before 'chat' must propagate through., Flags placed after 'chat' must still work. (+4 more)

### Community 174 - "test_doctor.py / TestDoctorMemoryProviderS"
Cohesion: 0.08
Nodes (12): Tests for hermes_cli.doctor., The ◆ Memory Provider section should respect memory.provider config., Create a minimal HERMES_HOME with config.yaml., Run doctor and capture stdout., Doctor should present CLI-gated tools as available in CLI context., test_run_doctor_sets_interactive_env_for_tool_checks(), test_run_doctor_termux_treats_docker_and_browser_warnings_as_expected(), TestDoctorMemoryProviderSection (+4 more)

### Community 175 - "test_mcp_tools_config.py / test_all_servers_disabled"
Cohesion: 0.07
Nodes (29): Tests for MCP tools interactive configuration in hermes_cli.tools_config., Tools in exclude list start unchecked., Only tools in include list start checked., Returns immediately when no MCP servers are configured., Each server gets its own checklist., Servers that fail to connect show warnings., Long descriptions are truncated in checklist labels., Returns immediately when all configured servers have enabled=false. (+21 more)

### Community 176 - "TestLongContextTierDetect / _is_long_context_tier_err"
Cohesion: 0.09
Nodes (13): _is_long_context_tier_error(), Tests for Anthropic Sonnet long-context tier 429 handling.  When Claude Max user, When the long-context tier error fires, context_length should     drop to 200k a, Verify the long-context 429 doesn't hit the generic rate-limit     or client-err, The error should be intercepted before the generic         is_rate_limited check, Opus should NOT match — falls through to generic rate-limit., A normal 429 should NOT match the long-context check., Verify the detection heuristic matches the Anthropic error. (+5 more)

### Community 177 - "test_slack_mention.py / _make_adapter()"
Cohesion: 0.14
Nodes (27): _make_adapter(), test_bot_uid_none_processes_channel_message(), test_channel_in_free_response_processed_without_mention(), test_default_require_mention_channel_without_mention_ignored(), test_dm_always_processed_regardless_of_setting(), test_free_response_channels_csv_string(), test_free_response_channels_default_empty(), test_free_response_channels_empty_string() (+19 more)

### Community 178 - "test_dingtalk.py / TestDeduplication"
Cohesion: 0.07
Nodes (8): Tests for DingTalk platform adapter., TestConnect, TestDeduplication, TestDingTalkAdapterInit, TestDingTalkRequirements, TestExtractText, TestPlatformEnum, TestSend

### Community 179 - "release.py / main()"
Cohesion: 0.1
Nodes (29): build_release_artifacts(), bump_version(), categorize_commit(), clean_subject(), generate_changelog(), get_commits(), get_current_version(), get_last_tag() (+21 more)

### Community 180 - "._resolve_chat_guid() / ._send_attachment()"
Cohesion: 0.09
Nodes (4): _normalize_server_url(), _redact(), _strip_markdown(), _value()

### Community 181 - "Button Design / Color Palette"
Cohesion: 0.4
Nodes (30): Button Design, Card Design, Color Palette, Components, Dark Theme, Gradient Usage, Layout System, Typography (+22 more)

### Community 182 - "fuzzy_match.py / _calculate_line_positions"
Cohesion: 0.1
Nodes (28): _apply_replacements(), _calculate_line_positions(), _find_normalized_matches(), fuzzy_find_and_replace(), _map_normalized_positions(), Apply replacements at the given positions.          Args:         content: Origi, Strategy 1: Exact string match., Strategy 2: Match with line-by-line whitespace trimming.          Strips leading (+20 more)

### Community 183 - "_compute_scroll_offset() / TestScrollOffsetLogic"
Cohesion: 0.1
Nodes (17): _compute_scroll_offset(), Tests for the scrolling viewport logic in _curses_prompt_choice (issue #5755)., Simulate pressing UP through all items; cursor always in view., Mirror of the scroll adjustment block inside _curses_menu., Return the list indices that would be rendered for the given state., Start position: offset stays 0, first items visible., Cursor inside the current window: offset unchanged., Cursor on Cancel (index 12) with 8-row window: offset = 12 - 8 + 1 = 5. (+9 more)

### Community 184 - "TestInterpretExitCode / test_terminal_exit_semant"
Cohesion: 0.07
Nodes (6): Tests for terminal command exit code semantic interpretation., Command with only env var assignments, no actual command., grep exit 2+ is a real error — should return None., Test _interpret_exit_code returns correct notes for known command semantics., In a pipeline, the last command determines the exit code., TestInterpretExitCode

### Community 185 - "test_telegram_commands.py / TestAuthorization"
Cohesion: 0.07
Nodes (9): E2E tests for Telegram gateway slash commands.  Each test drives a message throu, Verify session state changes across command sequences., Verify the pipeline handles unauthorized users., Verify the pipeline handles send failures gracefully., Gateway slash commands dispatched through the full adapter pipeline., TestAuthorization, TestSendFailureResilience, TestSessionLifecycle (+1 more)

### Community 186 - "adapter_factory() / test_telegram_reply_mode."
Cohesion: 0.12
Nodes (10): adapter_factory(), _ensure_telegram_mock(), test_all_mode_all_chunks_thread(), test_first_mode_only_first_chunk_threads(), test_no_reply_to_param_no_threading(), test_off_mode_no_reply_threading(), test_single_chunk_respects_mode(), TestEnvVarOverride (+2 more)

### Community 187 - "_new_check_escapes() / _old_check_escapes()"
Cohesion: 0.1
Nodes (19): _can_symlink(), _new_check_escapes(), _old_check_escapes(), Tests for the symlink boundary check prefix confusion fix in skills_guard.py.  R, Check if we can create symlinks (needs admin/dev-mode on Windows)., Test the full symlink scenario with real filesystem symlinks., A symlink from axolotl/ to axolotl-backdoor/ must be caught., A symlink that stays within the skill directory is fine. (+11 more)

### Community 188 - "TestSkillScopedPassthroug / test_env_passthrough.py"
Cohesion: 0.07
Nodes (11): _clean_passthrough(), Tests for tools.env_passthrough — skill and config env var passthrough., Verify that the passthrough is checked in execute_code's env filtering., TENOR_API_KEY should be blocked without passthrough., TENOR_API_KEY should pass through when registered., Verify that the passthrough is checked in terminal's env sanitizers., Ensure a clean passthrough state for every test., TestConfigPassthrough (+3 more)

### Community 189 - "._make_cli() / TestCLIPersonalityNone"
Cohesion: 0.12
Nodes (9): Tests for /personality none — clearing personality overlay., Test dict-format custom personalities with description, tone, style., test_default_clears_ephemeral_prompt(), test_list_includes_none(), test_none_clears_ephemeral_prompt(), test_unknown_shows_none_in_available(), TestCLIPersonalityNone, TestGatewayPersonalityNone (+1 more)

### Community 190 - "test_update_command.py / _make_runner()"
Cohesion: 0.16
Nodes (24): _make_event(), _make_runner(), test_cleans_up_files_after_notification(), test_cleans_up_on_error(), test_defers_notification_while_update_still_running(), test_fallback_to_sys_executable(), test_fallback_when_no_setsid(), test_handles_corrupt_pending_file() (+16 more)

### Community 191 - "_make_args() / test_webhook_cli.py"
Cohesion: 0.12
Nodes (7): _make_args(), Tests for hermes_cli/webhook.py — webhook subscription CLI., TestList, TestPersistence, TestRemove, TestSubscribe, TestWebhookEnabledGate

### Community 192 - "test_cli_provider_resolut / _import_cli()"
Cohesion: 0.11
Nodes (21): _import_cli(), _install_prompt_toolkit_stubs(), When provider resolves to openai-codex and no model was explicitly     chosen, t, Save and restore tools/cli/run_agent modules around every test., Model comes from config.yaml, not LLM_MODEL env var.     Config.yaml is the sing, When the user sets model.default in config.yaml to a specific codex     model, _, If the user explicitly passes a Codex-compatible model, it must be     preserved, openai/gpt-5.3-codex should become gpt-5.3-codex — the Codex     Responses API d (+13 more)

### Community 193 - "TestCLIQuickCommands / ._make_cli()"
Cohesion: 0.12
Nodes (13): _printed_plain(), Tests for user-defined quick commands that bypass the agent loop., Test quick command dispatch in HermesCLI.process_command., Test quick command dispatch in GatewayRunner._handle_message., Alias quick commands rewrite to the target command., Alias quick commands forward user arguments to the target., Quick commands must be checked before skill slash commands., test_exec_command_returns_output() (+5 more)

### Community 194 - "_make_agent() / test_flush_memories_codex"
Cohesion: 0.11
Nodes (17): _chat_response_with_memory_call(), _FakeOpenAI, _make_agent(), Tests for flush_memories() working correctly across all provider modes.  Catches, When auxiliary client is unavailable and we fall back to direct         OpenAI c, When an auxiliary client is available, flush_memories should use it     instead, Non-Codex mode with no auxiliary falls back to self.client., Verify that memory tool calls from the flush response actually get executed. (+9 more)

### Community 195 - "test_discord_reply_mode.p / TestEnvVarOverride"
Cohesion: 0.12
Nodes (12): adapter_factory(), _ensure_discord_mock(), _make_discord_adapter(), test_all_mode_all_chunks_reference(), test_first_mode_only_first_chunk_references(), test_invalid_mode_falls_back_to_first_behavior(), test_no_reply_to_param_no_reference(), test_off_mode_no_reply_reference() (+4 more)

### Community 196 - "test_discord_free_respons / make_message()"
Cohesion: 0.17
Nodes (21): _ensure_discord_mock(), FakeDMChannel, FakeForumChannel, FakeTextChannel, FakeThread, make_message(), test_discord_accepts_and_strips_bot_mentions_when_required(), test_discord_auto_thread_can_be_disabled() (+13 more)

### Community 197 - "send_message_tool.py / _error()"
Cohesion: 0.2
Nodes (25): _check_send_message(), _describe_media_for_mirror(), _error(), _get_cron_auto_delivery_target(), _handle_list(), _handle_send(), _maybe_skip_cron_duplicate_send(), _parse_target_ref() (+17 more)

### Community 198 - "TestManagedServerAPI / TestParserCompatibility"
Cohesion: 0.08
Nodes (16): Tests for ManagedServer / tool-parser integration.  Validates that: 1. The insta, ManagedServer checks `if parsed_tool_calls:` — None should be falsy., ManagedServer uses `parsed_content or ""` — must be str or None., Test that hermes_base_env.py's tool-parser wiring matches the current API., Hermes wires parser selection through ServerManager.tool_parser., Verify hermes_base_env uses the config field rather than a local parser instance, Test that ManagedServer's API matches what hermes-agent expects., ManagedServer should accept tool_call_parser parameter. (+8 more)

### Community 199 - "test_search_hidden_dirs.p / TestFindExcludesHiddenDir"
Cohesion: 0.08
Nodes (16): Tests that search_files excludes hidden directories by default.  Regression for, _write_index_cache should create .ignore in .hub/ directory., Create a directory tree with hidden and visible directories., _search_files uses find, which should exclude hidden directories., find should not return files from .hub/ directory., find should not return files from .git/ directory., find should still return files from visible directories., _search_with_grep should exclude hidden directories. (+8 more)

### Community 200 - "test_setup.py / _stub_tts()"
Cohesion: 0.13
Nodes (23): _clear_provider_env(), _maybe_keep_current_tts(), Tests for setup_model_provider — verifies the delegation to select_provider_and_, Nous OAuth writes config to disk; wizard config dict must pick it up., custom_providers written by select_provider_and_model must survive., When the user cancels provider selection, existing config is preserved., If select_provider_and_model raises, setup continues with existing config., KeyboardInterrupt during provider selection is handled. (+15 more)

### Community 201 - "test_tools_disable_enable / TestToolsValidation"
Cohesion: 0.08
Nodes (8): Tests for hermes tools disable/enable/list command (backend)., TestToolsDisableBuiltin, TestToolsDisableMcp, TestToolsEnableBuiltin, TestToolsEnableMcp, TestToolsList, TestToolsMixedTargets, TestToolsValidation

### Community 202 - "TestGenerateTitle / TestAutoTitleSession"
Cohesion: 0.08
Nodes (10): Tests for agent.title_generator — auto-generated session titles., Tests for maybe_auto_title() — the fire-and-forget entry point., Should not fire for conversations with more than 2 user messages., Should fire a background thread for the first exchange., Unit tests for generate_title()., Long user/assistant messages should be truncated in the LLM request., Tests for auto_title_session() — the sync worker function., TestAutoTitleSession (+2 more)

### Community 203 - "TestDiscordBotFilter / _make_author()"
Cohesion: 0.14
Nodes (16): _make_author(), _make_message(), Tests for Discord bot message filtering (DISCORD_ALLOW_BOTS)., Create a mock Discord author., Default behavior (no env var) should be 'none'., Allow_bots value should be case-insensitive., Create a mock Discord message., Test the DISCORD_ALLOW_BOTS filtering logic. (+8 more)

### Community 204 - "_make_message() / TestDiscordSystemMessageF"
Cohesion: 0.13
Nodes (16): _make_author(), _make_message(), Tests for Discord system message filtering (thread renames, pins, etc.)., Create a mock Discord author., Create a mock Discord message with a specific type., Test that Discord system messages (thread renames, pins, etc.) are ignored., Simulate the on_message filter logic and return whether message was accepted., Regular user messages (type=default) should be accepted. (+8 more)

### Community 205 - "TestCacheDocumentFromByte / test_document_cache.py"
Cohesion: 0.08
Nodes (9): Tests for document cache utilities in gateway/platforms/base.py.  Covers: get_do, Point the module-level DOCUMENT_CACHE_DIR to a fresh tmp_path., Malicious directory components are stripped — only the leaf name survives., A filename that is literally '..' falls back to 'document'., _redirect_cache(), TestCacheDocumentFromBytes, TestCleanupDocumentCache, TestGetDocumentCacheDir (+1 more)

### Community 206 - "TestSmsFormatAndTruncate / TestSmsToolset"
Cohesion: 0.1
Nodes (4): TestSmsConfigLoading, TestSmsFormatAndTruncate, TestSmsRequirements, TestSmsToolset

### Community 207 - "test_webhook_adapter.py / _make_adapter()"
Cohesion: 0.18
Nodes (23): _create_app(), _make_adapter(), _make_config(), test_concurrent_webhooks_get_independent_sessions(), test_connect_starts_server(), test_delivery_info_pruned_via_ttl(), test_delivery_info_survives_multiple_sends(), test_disconnect_cleans_up() (+15 more)

### Community 208 - "polymarket.py / _get()"
Cohesion: 0.17
Nodes (25): cmd_book(), cmd_event(), cmd_history(), cmd_market(), cmd_price(), cmd_search(), cmd_trades(), cmd_trending() (+17 more)

### Community 209 - "TestSanitizeTitle / Tests for SessionDB.sanit"
Cohesion: 0.08
Nodes (4): Tests for SessionDB.sanitize_title() validation and cleaning., set_session_title applies sanitize_title internally., set_session_title raises ValueError for overly long titles., TestSanitizeTitle

### Community 210 - "test_model_normalize.py / TestAggregatorProviders"
Cohesion: 0.08
Nodes (13): Tests for hermes_cli.model_normalize — provider-aware model name normalization., OpenCode Go model names with dots must pass through unchanged., opencode-go must NOT be in the dot-to-hyphen provider set., Anthropic API still needs dots→hyphens., OpenCode Zen follows Anthropic convention (dots→hyphens)., Copilot preserves dots in model names., Aggregators need vendor/model slugs., TestAggregatorProviders (+5 more)

### Community 211 - "_write_config() / TestNormalizeVisionProvid"
Cohesion: 0.11
Nodes (11): _isolate(), Tests for named custom provider and 'main' alias resolution in auxiliary_client., resolve_provider_client should resolve named custom providers directly., Redirect HERMES_HOME and clear module caches., Write a config.yaml to the test HERMES_HOME., _normalize_vision_provider should resolve 'main' to actual main provider., resolve_provider_client('main', ...) should resolve to actual main provider., TestNormalizeVisionProvider (+3 more)

### Community 212 - "test_models_dev.py / TestExtractContext"
Cohesion: 0.08
Nodes (5): Tests for agent.models_dev — models.dev registry integration., TestExtractContext, TestFetchModelsDev, TestLookupModelsDevContext, TestProviderMapping

### Community 213 - "_run() / test_youtube_quiz.py"
Cohesion: 0.12
Nodes (13): Tests for optional-skills/productivity/memento-flashcards/scripts/youtube_quiz.p, Handle plain list segments (no to_raw_data method)., Run main() with given argv and return parsed JSON output., When youtube-transcript-api is not installed, report the error., Create a mock youtube_transcript_api module., _run(), TestFetchMissingDependency, TestFetchWithMockedAPI (+5 more)

### Community 214 - "TRL Fine-tuning - Transfo / Training Acceleration - S"
Cohesion: 0.12
Nodes (25): Dataset Preparation - Data Formatting and Validation, Distributed Training - Multi-GPU/Multi-Node Training, Hyperparameter Tuning - Configuration Optimization, Inference Optimization - Deployment Speed, Model Checkpointing - Training Checkpoints, Quantization - Model Size Reduction, Reward Functions - Custom Reward Modeling, Tokenizers - Text Tokenization Strategies (+17 more)

### Community 215 - "TestWriteDenyExactPaths / TestWriteDenyPrefixes"
Cohesion: 0.08
Nodes (4): Tests for _is_write_denied() — verifies deny list blocks sensitive paths on all, TestWriteAllowed, TestWriteDenyExactPaths, TestWriteDenyPrefixes

### Community 216 - "test_feishu_approval_butt / _make_adapter()"
Cohesion: 0.16
Nodes (23): _ensure_feishu_mocks(), _make_adapter(), _make_card_action_data(), Tests for Feishu interactive card approval buttons., Provide stubs for lark-oapi / aiohttp.web so the import succeeds., Create a FeishuAdapter with mocked internals., Create a mock Feishu card action callback data object., test_already_resolved_drops_silently() (+15 more)

### Community 217 - "TestBuildStickerInjection / test_sticker_cache.py"
Cohesion: 0.08
Nodes (6): Tests for gateway/sticker_cache.py — sticker description cache., set_name alone (no emoji) produces no context — only emoji+set_name triggers 'fr, TestBuildAnimatedStickerInjection, TestBuildStickerInjection, TestCacheSticker, TestLoadSaveCache

### Community 218 - "_setup_sessions() / TestFindSessionId"
Cohesion: 0.11
Nodes (9): Tests for gateway/mirror.py — session mirroring., Helper to write a fake sessions.json and patch module-level paths., Verify _append_to_sqlite closes the SessionDB connection., Verify connection is closed even when append_message raises., _setup_sessions(), TestAppendToJsonl, TestAppendToSqlite, TestFindSessionId (+1 more)

### Community 219 - "test_discord_channel_cont / FakeTextChannel"
Cohesion: 0.18
Nodes (19): _ensure_discord_mock(), FakeDMChannel, FakeTextChannel, FakeThread, make_message(), test_config_bridges_ignored_channels(), test_config_bridges_no_thread_channels(), test_config_env_var_takes_precedence() (+11 more)

### Community 220 - "usage_pricing.py / get_pricing_entry()"
Cohesion: 0.14
Nodes (19): BillingRoute, CostResult, estimate_cost_usd(), estimate_usage_cost(), get_pricing(), get_pricing_entry(), has_known_pricing(), _lookup_official_docs_pricing() (+11 more)

### Community 221 - "providers.py / get_provider()"
Cohesion: 0.13
Nodes (21): determine_api_mode(), get_label(), get_overlay(), get_provider(), HermesOverlay, is_aggregator(), normalize_provider(), ProviderDef (+13 more)

### Community 222 - "_make_response() / test_browser_content_none"
Cohesion: 0.11
Nodes (14): _make_response(), Tests for None guard on browser_tool LLM response content.  browser_tool.py has, Build a minimal OpenAI-compatible ChatCompletion response stub., When LLM returns None content, should fall back to truncated snapshot., Normal string content should pass through., Empty string content should also fall back to truncated., tools/browser_tool.py — browser_vision() analysis extraction, When LLM returns None content, analysis should have a fallback message. (+6 more)

### Community 223 - "TestSanitizeEnvLines / .test_adds_missing_traili"
Cohesion: 0.09
Nodes (12): Tests for .env file corruption repair., Two KEY=VALUE pairs jammed on one line get split., A well-formed .env file passes through unchanged (modulo trailing newlines)., Lines missing trailing newline get one added., Three known keys on one line all get separated., A value containing '=' shouldn't be falsely split (lowercase in value)., Unknown key names on one line are NOT split (avoids false positives)., Concatenation is detected even when value ends with digits. (+4 more)

### Community 224 - "test_auth_commands.py / _write_auth_store()"
Cohesion: 0.15
Nodes (18): _jwt_with_email(), Tests for auth subcommands backed by the credential pool., Removing an env-seeded credential should also clear the env var from .env     so, After removing an env-seeded credential, load_pool should NOT re-create it., Removing a manually-added credential should NOT touch .env., test_auth_add_anthropic_oauth_persists_pool_entry(), test_auth_add_api_key_persists_manual_entry(), test_auth_add_codex_oauth_persists_pool_entry() (+10 more)

### Community 225 - "_simulate_config_bridge() / TestTopLevelCwdAlias"
Cohesion: 0.14
Nodes (9): Tests for the config.yaml → env var bridge logic in gateway/run.py.  Specificall, cwd: '.' should trigger MESSAGING_CWD fallback., MESSAGING_CWD in initial env should be picked up as fallback., Explicit top-level cwd should take precedence over MESSAGING_CWD., Simulate the gateway config bridge logic from gateway/run.py.      Returns the r, Top-level `cwd:` should be treated as `terminal.cwd`., terminal.cwd should win over top-level cwd., _simulate_config_bridge() (+1 more)

### Community 226 - "test_hooks.py / _patch_no_builtins()"
Cohesion: 0.14
Nodes (12): _create_hook(), _patch_no_builtins(), Tests for gateway/hooks.py — event hook system., Helper to create a hook directory with HOOK.yaml and handler.py., Suppress built-in hook registration so tests only exercise user-hook discovery., test_emit_calls_sync_handler(), test_emit_default_context(), test_handler_error_does_not_propagate() (+4 more)

### Community 227 - "TestQueryOllamaNumCtx / _mock_httpx_client()"
Cohesion: 0.12
Nodes (13): _mock_httpx_client(), Tests for Ollama num_ctx context length detection and injection.  Covers:   agen, Different model architectures use different key prefixes in model_info., Should return None if model_info has no context_length key., Create a mock httpx.Client context manager that returns given /api/show data., Test the Ollama /api/show context length query., Should extract context_length from GGUF model_info metadata., If the Modelfile sets num_ctx explicitly, that should take priority. (+5 more)

### Community 228 - "TestGetExternalSkillsDirs / test_external_skills.py"
Cohesion: 0.09
Nodes (10): external_skills_dir(), hermes_home(), Tests for external skill directories (skills.external_dirs config)., If the same skill name exists locally and externally, local wins., Create a temp dir with a sample external skill., Create a minimal HERMES_HOME with config., TestExternalSkillsInFindAll, TestExternalSkillView (+2 more)

### Community 229 - "test_google_oauth_setup.p / TestExchangeAuthCode"
Cohesion: 0.1
Nodes (8): FakeCredentials, FakeFlow, Regression tests for Google Workspace OAuth setup.  These tests cover the headle, Partial scopes are accepted with a warning (gws migration: v2.0)., reset(), setup_module(), TestExchangeAuthCode, TestGetAuthUrl

### Community 230 - "context_references.py / _expand_file_reference()"
Cohesion: 0.19
Nodes (20): _build_folder_listing(), _code_fence_language(), ContextReference, ContextReferenceResult, _ensure_reference_path_allowed(), _expand_file_reference(), _expand_folder_reference(), _expand_git_reference() (+12 more)

### Community 231 - "_path_escapes_skill_dir() / TestSkillViewPathBoundary"
Cohesion: 0.13
Nodes (14): _path_escapes_skill_dir(), Tests for the skill_view path boundary check.  Regression test: the original che, Reproduce the boundary check from tools/skills_tool.py.      Returns True when t, Verify the path boundary check works on all platforms., A file inside the skill directory must NOT be flagged., Deeply nested valid paths must also pass., A file outside the skill directory must be flagged., A file in a sibling skill directory must be flagged.          This catches prefi (+6 more)

### Community 232 - "TestApplyAnthropicCacheCo / TestApplyCacheMarker"
Cohesion: 0.1
Nodes (6): Tests for agent/prompt_caching.py — Anthropic cache control injection., Native Anthropic path: cache_control injected top-level (adapter moves it inside, OpenRouter path: top-level cache_control on role:tool is invalid and causes sile, Empty text blocks cannot have cache_control (Anthropic rejects them)., TestApplyAnthropicCacheControl, TestApplyCacheMarker

### Community 233 - "_make_agent() / TestFallbackChainAdvancem"
Cohesion: 0.18
Nodes (8): _make_agent(), _mock_client(), Tests for ordered provider fallback chain (salvage of PR #1761).  Extends the si, If resolve_provider_client returns None, skip to next in chain., Create a minimal AIAgent with optional fallback config., If resolve_provider_client raises, skip to next in chain., TestFallbackChainAdvancement, TestFallbackChainInit

### Community 234 - "TestBuildSessionContextPr / _make_context()"
Cohesion: 0.15
Nodes (3): _make_context(), TestBuildSessionContextPromptRedaction, TestHashHelpers

### Community 235 - "StubAdapter / test_platform_reconnect.p"
Cohesion: 0.19
Nodes (14): _make_runner(), StubAdapter, test_adapter_create_returns_none(), test_no_failed_platforms_watcher_idles(), test_nonretryable_error_triggers_shutdown(), test_nonretryable_runtime_error_not_queued(), test_reconnect_gives_up_after_max_attempts(), test_reconnect_nonretryable_removed_from_queue() (+6 more)

### Community 236 - "install.ps1 / Main()"
Cohesion: 0.34
Nodes (20): Copy-ConfigTemplates(), Install-Dependencies(), Install-NodeDeps(), Install-Repository(), Install-SystemPackages(), Install-Uv(), Install-Venv(), Invoke-SetupWizard() (+12 more)

### Community 237 - "cronjob_tools.py / cronjob()"
Cohesion: 0.16
Nodes (19): _canonical_skills(), check_cronjob_requirements(), cronjob(), _format_job(), list_cronjobs(), _normalize_optional_job_value(), _origin_from_env(), Cron job management tools for Hermes Agent.  Expose a single compressed action-o (+11 more)

### Community 238 - "model_normalize.py / normalize_model_for_provi"
Cohesion: 0.14
Nodes (19): detect_vendor(), _dots_to_hyphens(), is_aggregator_provider(), model_display_name(), _normalize_for_deepseek(), normalize_model_for_provider(), _prepend_vendor(), Per-provider model name normalization.  Different LLM providers expect model ide (+11 more)

### Community 239 - "TestCliSkinPromptIntegrat / _make_cli_stub()"
Cohesion: 0.15
Nodes (4): _make_cli_stub(), TestAnsiRichTextHelper, TestCliSkinPromptIntegration, TestCompactBannerSkinIntegration

### Community 240 - "TestEnsureSingularityAvai / TestFindSingularityExecut"
Cohesion: 0.1
Nodes (12): Tests for Singularity/Apptainer preflight availability check.  Verifies that a c, _find_singularity_executable resolution tests., When both are available, apptainer should be preferred., When only singularity is available, use it., Must raise RuntimeError with install instructions., _ensure_singularity_available preflight tests., Returns the executable name when version check passes., Raises RuntimeError when version command fails. (+4 more)

### Community 241 - "test_slack_approval_butto / _make_adapter()"
Cohesion: 0.18
Nodes (16): _ensure_slack_mock(), _make_adapter(), test_api_failure_returns_empty(), test_bot_message_ts_cap(), test_deny_action(), test_empty_thread(), test_fetches_and_formats_context(), test_not_connected() (+8 more)

### Community 242 - "test_discord_document_han / make_message()"
Cohesion: 0.26
Nodes (17): _ensure_discord_mock(), FakeDMChannel, make_attachment(), make_message(), _mock_aiohttp_download(), _redirect_cache(), test_download_error_handled(), test_image_attachment_unaffected() (+9 more)

### Community 243 - "test_telegram_reactions.p / _make_adapter()"
Cohesion: 0.21
Nodes (19): _make_adapter(), _make_event(), test_config_bridges_telegram_reactions(), test_config_reactions_env_takes_precedence(), test_on_processing_complete_failure(), test_on_processing_complete_skipped_when_disabled(), test_on_processing_complete_success(), test_on_processing_start_adds_eyes_reaction() (+11 more)

### Community 244 - "TestMergeCaptionBasic / TestMergeCaptionSubstring"
Cohesion: 0.1
Nodes (6): Tests for TelegramPlatform._merge_caption caption deduplication logic., These are the exact scenarios that the old substring check got wrong., TestMergeCaptionBasic, TestMergeCaptionMultipleItems, TestMergeCaptionSubstringBug, TestMergeCaptionWhitespace

### Community 245 - "test_matrix_voice.py / _make_audio_event()"
Cohesion: 0.17
Nodes (15): _make_adapter(), _make_audio_event(), _make_download_response(), _make_room(), Tests for Matrix voice message support (MSC3245)., Create a MatrixAdapter with mocked config., Create a mock Matrix room., Create a mock RoomMessageAudio event that passes isinstance checks.          Arg (+7 more)

### Community 246 - "TestSSEAgentCancelOnDisco / _make_adapter()"
Cohesion: 0.13
Nodes (12): _make_adapter(), _make_request(), Tests for SSE client disconnect → agent task cancellation.  When a streaming /v1, BrokenPipeError (another disconnect variant) also cancels the task., If agent already finished before disconnect, don't try to cancel., When the client disconnects, agent.interrupt() must be called         so the age, Build a minimal APIServerAdapter with mocked internals., When agent_ref is not provided (None), the task is still cancelled         on di (+4 more)

### Community 247 - "TestConfigFilePermissions / test_file_permissions.py"
Cohesion: 0.1
Nodes (7): Tests for file permissions hardening on sensitive files., Test the _secure_file and _secure_dir helpers., Verify cron files get secure permissions., Verify config files get secure permissions., TestConfigFilePermissions, TestCronFilePermissions, TestSecureHelpers

### Community 248 - "skill_commands.py / build_skill_invocation_me"
Cohesion: 0.14
Nodes (19): build_plan_path(), build_preloaded_skills_prompt(), build_skill_invocation_message(), _build_skill_message(), get_skill_commands(), _inject_skill_config(), _load_skill_payload(), Shared slash command helpers for skills and built-in prompt-style modes.  Shared (+11 more)

### Community 249 - "basic_grpo_training.py / main()"
Cohesion: 0.13
Nodes (19): correctness_reward_func(), extract_answer(), extract_xml_tag(), format_reward_func(), get_dataset(), get_peft_config(), incremental_format_reward_func(), main() (+11 more)

### Community 250 - "Instructor / NeMo Curator"
Cohesion: 0.12
Nodes (20): Anthropic Claude, Automatic Retry on Validation, Dask Distributed Computing, GPU-Accelerated Data Curation, Fuzzy Deduplication, GPU-Based Training, Real-World Extraction Examples, LLM Provider Configuration (+12 more)

### Community 251 - "TestProbeMcpServerTools / test_mcp_probe.py"
Cohesion: 0.11
Nodes (10): Tests for probe_mcp_server_tools() in tools.mcp_tool., Ensure clean MCP module state before/after each test., Tools without descriptions get empty string., _stop_mcp_loop is called even when probe fails., Disabled servers are not probed., Tests for the lightweight probe_mcp_server_tools function., Successfully probed server returns its tools list., Servers that fail to connect are silently skipped. (+2 more)

### Community 252 - "TestFuzzyPatchSkill / test_skill_improvements.p"
Cohesion: 0.11
Nodes (8): Tests for skill fuzzy patching via tools.fuzzy_match., Fuzzy matching should also work on supporting files., Fuzzy matching should still run frontmatter validation on SKILL.md., The dispatcher should route to the fuzzy-matching patch., Patch with extra leading whitespace should still find the target., Patch where only indentation differs should succeed., Multiple fuzzy matches should return an error without replace_all., TestFuzzyPatchSkill

### Community 253 - "TestExpandEnvVars / test_config_env_expansion"
Cohesion: 0.11
Nodes (5): Tests for ${ENV_VAR} substitution in config.yaml values., Verify that load_cli_config() also expands ${VAR} references., TestExpandEnvVars, TestLoadCliConfigExpansion, TestLoadConfigExpansion

### Community 254 - "_run() / test_daytona_terminal.py"
Cohesion: 0.15
Nodes (9): Integration tests for the Daytona terminal backend.  Requires DAYTONA_API_KEY to, Provide a unique task_id and clean up the sandbox after the test., Write a file, stop the sandbox, resume it, assert the file persists., _run(), task_id(), TestDaytonaBasic, TestDaytonaFilesystem, TestDaytonaIsolation (+1 more)

### Community 255 - "TestExtractImages / .test_non_image_ext_not_e"
Cohesion: 0.11
Nodes (1): TestExtractImages

### Community 256 - "TestResetPolicyNotify / TestShouldResetReason"
Cohesion: 0.19
Nodes (5): _make_source(), _make_store(), TestResetPolicyNotify, TestSessionEntryReason, TestShouldResetReason

### Community 257 - "google_api.py / gws()"
Cohesion: 0.19
Nodes (17): calendar_create(), calendar_delete(), calendar_list(), contacts_list(), docs_get(), drive_search(), gmail_get(), gmail_labels() (+9 more)

### Community 258 - "script.js / TerminalDemo"
Cohesion: 0.15
Nodes (3): switchPlatform(), switchStepPlatform(), TerminalDemo

### Community 259 - "Conference Paper Checklis / Research Paper Writing Sk"
Cohesion: 0.11
Nodes (19): ACL Conference, Conference Paper Checklists, Citation Hallucination Prevention, Citation Management & Hallucination Prevention, CrossRef API, Ethics & Broader Impact, Experiment Infrastructure & Design, Experiment Design Patterns (+11 more)

### Community 260 - "TestSafeWriteRoot / TestStaticDenyList"
Cohesion: 0.11
Nodes (7): Tests for file write safety and HERMES_WRITE_SAFE_ROOT sandboxing.  Based on PR, Basic sanity checks for the static write deny list., HERMES_WRITE_SAFE_ROOT should sandbox writes to a specific subtree., ~ in HERMES_WRITE_SAFE_ROOT should be expanded., Even if a static-denied path is inside the safe root, it's still denied., TestSafeWriteRoot, TestStaticDenyList

### Community 261 - "TestProviderPersistsAfter / test_model_provider_persi"
Cohesion: 0.11
Nodes (10): config_home(), Tests that provider selection via `hermes model` always persists correctly.  Reg, _model_flow_copilot should persist provider/base_url/model together., _model_flow_copilot_acp should persist provider/base_url/model together., Isolated HERMES_HOME with a minimal string-format config., When config.model is a plain string, _save_model_choice must         convert it, When config.model is already a dict, _save_model_choice preserves it., _model_flow_api_key_provider must persist the provider even when         config. (+2 more)

### Community 262 - "TestFormatSessionInfo / _patch_info()"
Cohesion: 0.16
Nodes (8): _patch_info(), Tests for GatewayRunner._format_session_info — session config surfacing., If runtime resolution raises, should still produce output., Create a bare GatewayRunner without __init__., Return a context-manager stack that patches _format_session_info deps., No config.yaml should not crash., runner(), TestFormatSessionInfo

### Community 263 - "ProgressCaptureAdapter / test_run_progress_topics."
Cohesion: 0.18
Nodes (9): _make_runner(), ProgressCaptureAdapter, _run_long_preview_helper(), test_all_mode_default_truncation_40_chars(), test_all_mode_no_truncation_when_preview_fits(), test_all_mode_respects_custom_preview_length(), test_run_agent_progress_does_not_use_event_message_id_for_telegram_dm(), test_run_agent_progress_stays_in_originating_topic() (+1 more)

### Community 264 - "_filter_history() / TestTranscriptHistoryOffs"
Cohesion: 0.15
Nodes (11): _filter_history(), Tests for transcript history offset fix.  Regression tests for a bug where the g, First turn has no session_meta, so both approaches agree., Two session_meta entries double the offset error.          This can happen when, system messages in history are also stripped from agent_history., When agent has fewer messages than offset, return [] not all.          The old c, Tool call messages pass through the filter, keeping offset correct., Replicate the agent_history filtering from GatewayRunner._run_agent.      Strips (+3 more)

### Community 265 - "TestPathTraversalBlocked / test_skill_view_traversal"
Cohesion: 0.12
Nodes (10): fake_skills(), Tests for path traversal prevention in skill_view.  Regression tests for issue #, Create a fake skills directory with one skill and a sensitive file outside., Direct .. traversal should be rejected., Nested .. traversal should also be rejected., Valid paths within the skill directory should work normally., Calling skill_view without file_path should return the SKILL.md., Symlinks pointing outside the skill directory should be blocked. (+2 more)

### Community 266 - "TestYoloMode / test_yolo_mode.py"
Cohesion: 0.12
Nodes (9): Tests for --yolo (HERMES_YOLO_MODE) approval bypass., Empty string for HERMES_YOLO_MODE should not trigger bypass., When HERMES_YOLO_MODE is set, all dangerous commands are auto-approved., Without yolo mode, dangerous commands in interactive mode require approval., With HERMES_YOLO_MODE, dangerous commands are auto-approved., Yolo mode bypasses all dangerous patterns, not just some., The new combined guard should preserve yolo bypass semantics., HERMES_YOLO_MODE should not be set by default. (+1 more)

### Community 267 - "test_auth_codex_provider. / _setup_hermes_auth()"
Cohesion: 0.16
Nodes (11): _jwt_with_exp(), Tests for Codex auth — tokens stored in Hermes auth store (~/.hermes/auth.json)., Verify Hermes never writes to ~/.codex/auth.json., Write Codex tokens into the Hermes auth store., _setup_hermes_auth(), test_codex_tokens_not_written_to_shared_file(), test_read_codex_tokens_success(), test_resolve_codex_runtime_credentials_force_refresh() (+3 more)

### Community 268 - "_make_cli() / TestMCPConfigWatch"
Cohesion: 0.16
Nodes (10): _make_cli(), Tests for automatic MCP reload when config.yaml mcp_servers section changes., If mtime and mcp_servers unchanged, _reload_mcp is NOT called., If file mtime changes but mcp_servers is identical, no reload., Adding a new MCP server to config triggers auto-reload., Removing an MCP server from config triggers auto-reload., Create a minimal HermesCLI instance with mocked config., If called within CONFIG_WATCH_INTERVAL, stat() is skipped. (+2 more)

### Community 269 - "TestBuildApiKwargs / Default reasoning config "
Cohesion: 0.12
Nodes (2): Default reasoning config for OpenRouter should be medium., TestBuildApiKwargs

### Community 270 - "TestToolUseEnforcementCon / ._make_agent()"
Cohesion: 0.2
Nodes (4): Tests for the agent.tool_use_enforcement config option., Create an agent with tools and a specific enforcement config., Even with enforcement=true, no injection when agent has no tools., TestToolUseEnforcementConfig

### Community 271 - "test_google_workspace_api / _write_token()"
Cohesion: 0.14
Nodes (14): Tests for Google Workspace gws bridge and CLI wrapper., Missing token file causes exit with code 1., main() sets GOOGLE_WORKSPACE_CLI_TOKEN in subprocess env., calendar list without dates uses +agenda helper., calendar list with --start/--end uses raw events list API., Non-expired token is returned without refresh., Expired token triggers a refresh via token_uri., test_api_calendar_list_respects_date_range() (+6 more)

### Community 272 - "DummyTelegramAdapter / test_base_topic_sessions."
Cohesion: 0.21
Nodes (8): DummyTelegramAdapter, _make_event(), test_handle_message_does_not_interrupt_different_topic(), test_handle_message_interrupts_same_topic(), test_process_message_background_marks_cancellation_unsuccessful(), test_process_message_background_marks_exception_unsuccessful(), test_process_message_background_marks_total_send_failure_unsuccessful(), test_process_message_background_replies_in_same_topic()

### Community 273 - "_make_adapter() / TestBlueBubblesHelpers"
Cohesion: 0.19
Nodes (3): _make_adapter(), TestBlueBubblesHelpers, TestBlueBubblesWebhookParsing

### Community 274 - "discord-voice-doctor.py / check_env_vars()"
Cohesion: 0.27
Nodes (16): check(), check_bot_permissions(), check_config(), check_env_vars(), check_packages(), check_system_tools(), main(), mask() (+8 more)

### Community 275 - "merge_runs.py / _merge_runs_in()"
Cohesion: 0.25
Nodes (16): _can_merge(), _consolidate_text(), _find_elements(), _first_child_run(), _get_child(), _get_children(), _is_adjacent(), _is_run() (+8 more)

### Community 276 - "stream_consumer.py / ._send_fallback_final()"
Cohesion: 0.15
Nodes (9): _clean_for_display(), Gateway streaming consumer — bridges sync agent callbacks to async platform deli, Async task that drains the queue and edits the platform message., Send a new message chunk, optionally threaded to a previous message.          Re, Return the visible text already shown in the streamed message., Return only the part of final_text the user has not already seen., Send the final continuation after streaming edits stop working., Send or edit the streaming message. (+1 more)

### Community 277 - "Sparse Autoencoder (SAE) / Simple Preference Optimiz"
Cohesion: 0.12
Nodes (17): SAE Analysis & Steering Workflow, Anthropic Monosemanticity Research, Feature Discovery in Neural Networks, Mechanistic Interpretability, Monosemanticity, SAELens Skill, Sparse Autoencoder (SAE), Superposition Phenomenon (+9 more)

### Community 278 - "env_passthrough.py / _get_allowed()"
Cohesion: 0.17
Nodes (15): clear_env_passthrough(), get_all_passthrough(), _get_allowed(), is_env_passthrough(), _load_config_passthrough(), Environment variable passthrough registry.  Skills that declare ``required_envir, Reset the skill-scoped allowlist (e.g. on session reset)., Force re-read of config on next access (for testing). (+7 more)

### Community 279 - "copilot_auth.py / resolve_copilot_token()"
Cohesion: 0.15
Nodes (15): copilot_device_code_login(), copilot_request_headers(), _gh_cli_candidates(), is_classic_pat(), GitHub Copilot authentication utilities.  Implements the OAuth device code flow, Return candidate ``gh`` binary paths, including common Homebrew installs., Return a token from ``gh auth token`` when the GitHub CLI is available., Run the GitHub OAuth device code flow for Copilot.      Prints instructions for (+7 more)

### Community 280 - "EvidenceStore / main()"
Cohesion: 0.25
Nodes (6): EvidenceStore, main(), _now_iso(), Re-compute SHA-256 for all entries and report mismatches., Search for keyword in content, source, actor, or url., _sha256()

### Community 281 - "test_managed_modal_enviro / _install_fake_tools_packa"
Cohesion: 0.26
Nodes (13): _FakeResponse, _install_fake_tools_package(), _load_tool_module(), Save and restore sys.modules entries so fakes don't leak to other tests., _reset_modules(), _restore_tool_and_agent_modules(), test_managed_modal_create_and_cleanup_preserve_gateway_persistence_fields(), test_managed_modal_create_sends_a_stable_idempotency_key() (+5 more)

### Community 282 - "_make_image() / test_cli_image_command.py"
Cohesion: 0.21
Nodes (6): _make_cli(), _make_image(), TestCollectQueryImages, TestImageBadgeFormatting, TestImageCommand, TestTermuxImageHints

### Community 283 - "test_anthropic_error_hand / _run_with_agent()"
Cohesion: 0.25
Nodes (14): _anthropic_response(), _fake_build_anthropic_client(), _FakeAnthropicClient, _make_agent_cls(), _patch_agent_bootstrap(), _run_with_agent(), test_400_bad_request_is_non_retryable(), test_401_credential_refresh_recovers() (+6 more)

### Community 284 - "extract_media_tags_fixed( / TestMediaExtraction"
Cohesion: 0.17
Nodes (11): extract_media_tags_broken(), extract_media_tags_fixed(), Tests for MEDIA tag extraction from tool results.  Verifies that MEDIA tags (e.g, MEDIA tags from the current turn SHOULD be extracted., Multiple TTS calls in history should NOT accumulate in new responses., Extract MEDIA tags from tool results, but ONLY from new messages     (those adde, Multiple MEDIA tags in current turn should be deduplicated., The BROKEN behavior: extract MEDIA tags from ALL messages including history. (+3 more)

### Community 285 - "test_command_bypass_activ / _make_adapter()"
Cohesion: 0.42
Nodes (15): _make_adapter(), _make_event(), _session_key(), test_approve_bypasses_guard(), test_deny_bypasses_guard(), test_file_path_not_treated_as_command(), test_new_bypasses_guard(), test_new_with_botname() (+7 more)

### Community 286 - "session_search_tool.py / session_search()"
Cohesion: 0.18
Nodes (14): check_session_search_requirements(), _format_conversation(), _format_timestamp(), _list_recent_sessions(), Summarize a single session conversation focused on the search query., Return metadata for the most recent sessions (no LLM calls)., Search past sessions and return focused summaries of matching conversations., Convert a Unix timestamp (float/int) or ISO string to a human-readable date. (+6 more)

### Community 287 - "TestExactMatch / test_fuzzy_match.py"
Cohesion: 0.13
Nodes (5): Tests for the fuzzy matching module., TestExactMatch, TestIndentDifference, TestReplaceAll, TestWhitespaceDifference

### Community 288 - "_new_should_allow() / TestPolicyPrecedenceForDa"
Cohesion: 0.21
Nodes (6): _new_should_allow(), _old_should_allow(), Regression tests for skills guard policy precedence.  Official/builtin skills sh, Simulate the BROKEN old logic., Simulate the FIXED logic., TestPolicyPrecedenceForDangerousVerdicts

### Community 289 - "_run_switch() / TestVariantTagPreservatio"
Cohesion: 0.18
Nodes (10): Tests for OpenRouter variant tag preservation in model switching.  Regression te, Run switch_model with mocked dependencies, return the resolved model name., OpenRouter variant tags (:free, :extended, :fast) must survive model switching., Legacy vendor:model (no slash) should still be converted to vendor/model., vendor:model:free (no slash) → vendor/model:free — first colon becomes slash., Bare model names without colons or slashes should work normally., Standard vendor/model slugs without tags pass through unchanged., _run_switch() (+2 more)

### Community 290 - "main() / test_modal_terminal.py"
Cohesion: 0.19
Nodes (14): main(), Test executing Python code in Modal., Test installing a package with pip in Modal., Test that filesystem persists between commands in the same task., Test that different task_ids get isolated environments., Run all Modal terminal tests., Test that Modal requirements are met., Test executing a simple command. (+6 more)

### Community 291 - "TestSaveConfigValueAtomic / test_cli_save_config_valu"
Cohesion: 0.13
Nodes (8): Tests for save_config_value() in cli.py — atomic write behavior., save_config_value() must use atomic_yaml_write to avoid data loss., save_config_value must route through atomic_yaml_write, not bare open()., Writing a new key must not clobber existing config entries., Dot-separated paths create intermediate dicts as needed., Updating an existing key replaces the value., If atomic_yaml_write raises, the original file is untouched., TestSaveConfigValueAtomic

### Community 292 - "test_background_command.p / _make_runner()"
Cohesion: 0.32
Nodes (14): _make_event(), _make_runner(), test_background_in_help_output(), test_bg_alias_no_prompt_shows_usage(), test_empty_prompt_shows_usage(), test_exception_sends_error_message(), test_no_adapter_returns_silently(), test_no_credentials_sends_error() (+6 more)

### Community 293 - "_RetryableFailureAdapter / _DisabledAdapter"
Cohesion: 0.15
Nodes (3): _DisabledAdapter, _RetryableFailureAdapter, test_runner_returns_failure_for_retryable_startup_errors()

### Community 294 - "_FakeRegistry / TestLoadBackgroundNotific"
Cohesion: 0.22
Nodes (7): _build_runner(), _FakeRegistry, test_no_thread_id_sends_no_metadata(), test_run_process_watcher_respects_notification_mode(), test_thread_id_passed_to_send(), TestLoadBackgroundNotificationsMode, _watcher_dict()

### Community 295 - "_FatalAdapter / _RuntimeRetryableAdapter"
Cohesion: 0.16
Nodes (4): _FatalAdapter, _RuntimeRetryableAdapter, test_runner_queues_retryable_runtime_fatal_for_reconnection(), test_runner_requests_clean_exit_for_nonretryable_startup_conflict()

### Community 296 - "telegram_network.py / discover_fallback_ips()"
Cohesion: 0.18
Nodes (12): discover_fallback_ips(), _is_retryable_connect_error(), _normalize_fallback_ips(), parse_fallback_ip_env(), _query_doh_provider(), Telegram-specific network helpers.  Provides a hostname-preserving fallback tran, Return the IPv4 addresses that the OS resolver gives for api.telegram.org., Query one DoH provider and return A-record IPs. (+4 more)

### Community 297 - "base / solana"
Cohesion: 0.18
Nodes (15): base, Base, Blockchain, Crypto, DeFi, Ethereum, EVM, L2 (+7 more)

### Community 298 - "llama.cpp: CPU/Apple Sili / MLOps Inference Skills Ca"
Cohesion: 0.18
Nodes (15): Finite State Machine (FSM) for Constrained Generation, GGUF Quantization, GGUF Quantization Types (K-quants), Guidance: Constrained LLM Generation, Hardware Acceleration (Metal/CUDA/ROCm), llama.cpp: CPU/Apple Silicon Inference, Mechanistic Interpretability, MLOps Inference Skills Category (+7 more)

### Community 299 - "Google Workspace Skill / Obsidian Note Taking Skil"
Cohesion: 0.13
Nodes (15): Gmail Search Operators, Calendar Service, Contacts Service, Google Docs Service, Google Drive Service, Gmail Service, Google Sheets Service, Google Workspace Skill (+7 more)

### Community 300 - "osv_check.py / check_package_for_malware"
Cohesion: 0.2
Nodes (13): check_package_for_malware(), _infer_ecosystem(), _parse_npm_package(), _parse_package_from_args(), _parse_pypi_package(), _query_osv(), OSV malware check for MCP extension packages.  Before launching an MCP server vi, Parse npm package: @scope/name@version or name@version. (+5 more)

### Community 301 - "domain_intel.py / bulk_check()"
Cohesion: 0.15
Nodes (13): bulk_check(), check_available(), check_ssl(), dns_records(), main(), Query WHOIS servers for domain registration info., Resolve DNS records using system DNS + Google DoH., Check domain availability using passive signals (DNS + WHOIS + SSL). (+5 more)

### Community 302 - "TestParseEnvVar / test_parse_env_var.py"
Cohesion: 0.14
Nodes (3): Tests for _parse_env_var and _get_env_config env-var validation., Unit tests for _parse_env_var., TestParseEnvVar

### Community 303 - "TestMarkdownStripping / _strip_markdown_for_tts d"
Cohesion: 0.14
Nodes (2): _strip_markdown_for_tts does NOT truncate — that's the caller's job., TestMarkdownStripping

### Community 304 - "TestBrowserCleanup / test_browser_cleanup.py"
Cohesion: 0.14
Nodes (5): Regression tests for browser session cleanup and screenshot recovery., When camofox mode + managed persistence, soft_cleanup fires instead of close., When camofox mode but managed persistence is off, camofox_close fires., TestBrowserCleanup, TestScreenshotPathRecovery

### Community 305 - "TestToolsetIntersection / test_delegate_toolset_sco"
Cohesion: 0.14
Nodes (8): Tests for delegate_tool toolset scoping.  Verifies that subagents cannot gain to, Subagent toolsets must be a subset of parent's enabled_toolsets., LLM requests toolsets parent doesn't have — extras are dropped., LLM requests subset of parent tools — all pass through., When toolsets is None/empty, child inherits parent's set., Blocked toolsets (delegation, clarify, etc.) are always removed., If parent has no overlap with requested, child gets nothing extra., TestToolsetIntersection

### Community 306 - "TestMultiWordInjectionByp / test_cron_prompt_injectio"
Cohesion: 0.14
Nodes (5): Regression tests for cron prompt injection scanner bypass.  The original regex `, Multi-word variants that previously bypassed the scanner., Original single-word patterns must still be caught., Ensure the broader regex doesn't create false positives., TestMultiWordInjectionBypass

### Community 307 - "_create_skill() / TestSkillViewRegistersPas"
Cohesion: 0.19
Nodes (8): _create_skill(), Test that skill_view registers required env vars in the passthrough registry., Skills without required_environment_variables shouldn't register anything., Create a minimal skill directory with SKILL.md., When a skill declares required_environment_variables and the var IS set,, Remote-backed skills still register locally available env vars., When a skill declares required_environment_variables but the var is NOT set,, TestSkillViewRegistersPassthrough

### Community 308 - "TestNonInteractiveSetup / test_setup_noninteractive"
Cohesion: 0.19
Nodes (9): _make_chat_args(), _make_setup_args(), Tests for non-interactive setup and first-run headless behavior., Verify setup paths exit cleanly in headless/non-interactive environments., --non-interactive should print guidance and not enter the wizard., When stdin has no TTY, the setup wizard should print guidance and return., Bare `hermes` should not prompt for input when no provider exists and stdin is h, Returning-user menu should map Terminal Backend to the terminal setup, not TTS. (+1 more)

### Community 309 - "test_context_references.p / _git()"
Cohesion: 0.15
Nodes (2): _git(), sample_repo()

### Community 310 - "TestStepCallbackNormaliza / ._extract_step_callback()"
Cohesion: 0.18
Nodes (8): Tests for step_callback backward compatibility.  Verifies that the gateway's ste, The documented hook example: ', '.join(tool_names) should work., The gateway's _step_callback_sync normalizes prev_tools from run_agent., Build a minimal _step_callback_sync using the same logic as gateway/run.py., When prev_tools is list[dict], tool_names should be list[str]., When prev_tools is list[str] (legacy), tool_names should pass through., Empty or None prev_tools should produce empty tool_names., TestStepCallbackNormalization

### Community 311 - "sticker_cache.py / cache_sticker_description"
Cohesion: 0.18
Nodes (13): build_animated_sticker_injection(), build_sticker_injection(), cache_sticker_description(), get_cached_description(), _load_cache(), Sticker description cache for Telegram.  When users send stickers, we describe t, Build injection text for animated/video stickers we can't analyze., Load the sticker cache from disk. (+5 more)

### Community 312 - "Memory Framework Architec / Semantic Search Pattern"
Cohesion: 0.21
Nodes (14): AI Provider Ecosystem, Fact Extraction & Memory Lifecycle, ByteRover Memory Provider, Memory Framework Architecture, Hindsight Memory Provider, Holographic Memory Provider, Honcho Memory Provider, Mem0 Memory Provider (+6 more)

### Community 313 - "Manim-Video/Skill / Manim-Video/References/An"
Cohesion: 0.14
Nodes (14): Animations Reference, Core Concept, Creation Animations, Creative Standard, Manim Video Production Pipeline, Modes, Prerequisites, Manim-Video/References/Animations (+6 more)

### Community 314 - "Claude Design System / Gemini Design System"
Cohesion: 0.57
Nodes (14): Bolt Design System, Claude Design System, Cohere Design System, Copilot Design System, Cursor Design System, FAL AI Design System, Gemini Design System, Grok Design System (+6 more)

### Community 315 - "Agent Loop Internals / Adding Tools"
Cohesion: 0.24
Nodes (14): ACP Internals, Adding Tools, Agent Loop Internals, Creating Skills, Automate Anything with Cron, Gateway Internals, Installation, Run Local LLMs on Mac (+6 more)

### Community 316 - "Caduceus Banner Section / CLI Terminal Window"
Cohesion: 0.15
Nodes (14): Agent Responses, Slash Command Autocomplete, Banner Details, HERMES AGENT Banner Icon, Banner Info Box (Left), Banner Info Box (Right), Caduceus Banner Section, CLI Terminal Window (+6 more)

### Community 317 - "test_evidence_store.py / test_evidence_store_add()"
Cohesion: 0.15
Nodes (0): 

### Community 318 - "_load_module() / test_browser_camofox_stat"
Cohesion: 0.22
Nodes (5): _load_module(), Tests for Hermes-managed Camofox state helpers., TestCamofoxConfigDefaults, TestCamofoxIdentity, TestCamofoxStatePaths

### Community 319 - "test_windows_compat.py / _get_preexec_fn_values()"
Cohesion: 0.17
Nodes (10): _get_preexec_fn_values(), Tests for Windows compatibility of process management code.  Verifies that os.se, Find all preexec_fn= keyword arguments in Popen calls., preexec_fn must never be a bare os.setsid reference., Each guarded file must define _IS_WINDOWS., os.killpg must always be behind a platform check., test_preexec_fn_is_guarded(), TestIsWindowsConstant (+2 more)

### Community 320 - "_clear_terminal_env() / test_terminal_requirement"
Cohesion: 0.27
Nodes (12): _clear_terminal_env(), Local backend uses Hermes' own LocalEnvironment wrapper., Remove terminal env vars that could affect requirements checks., test_local_terminal_requirements(), test_modal_backend_auto_mode_prefers_managed_gateway_over_direct_creds(), test_modal_backend_direct_mode_does_not_fall_back_to_managed(), test_modal_backend_managed_mode_does_not_fall_back_to_direct(), test_modal_backend_managed_mode_without_feature_flag_logs_clear_error() (+4 more)

### Community 321 - "TestToOpenaiBaseUrl / test_minimax_auxiliary_ur"
Cohesion: 0.15
Nodes (3): Tests for MiniMax auxiliary client URL normalization.  MiniMax and MiniMax-CN se, api.anthropic.com doesn't end with /anthropic — should be untouched., TestToOpenaiBaseUrl

### Community 322 - "StubAdapter / test_interrupt_key_match."
Cohesion: 0.26
Nodes (6): _source(), StubAdapter, test_get_pending_message_requires_session_key(), test_handle_message_stores_under_session_key(), test_has_pending_interrupt_requires_session_key(), test_photo_followup_is_queued_without_interrupt()

### Community 323 - "test_whatsapp_group_gatin / _make_adapter()"
Cohesion: 0.37
Nodes (11): _group_message(), _make_adapter(), test_dm_always_passes_even_with_require_mention(), test_free_response_chats_bypass_mention_gating(), test_free_response_chats_does_not_bypass_other_groups(), test_group_messages_can_be_opened_via_config(), test_group_messages_can_require_direct_trigger_via_config(), test_invalid_regex_patterns_are_ignored() (+3 more)

### Community 324 - "test_approve_deny_command / _make_event()"
Cohesion: 0.47
Nodes (12): _make_event(), _make_runner(), _make_source(), test_approve_all_resolves_multiple(), test_approve_all_session(), test_approve_no_pending(), test_approve_resolves_blocking_approval(), test_approve_stale_old_style_pending() (+4 more)

### Community 325 - "test_telegram_approval_bu / _make_adapter()"
Cohesion: 0.28
Nodes (12): _ensure_telegram_mock(), _make_adapter(), test_already_resolved(), test_deny_button(), test_model_picker_callback_not_affected(), test_not_connected(), test_resolves_approval_on_click(), test_sends_in_thread() (+4 more)

### Community 326 - "test_title_command.py / _make_event()"
Cohesion: 0.41
Nodes (12): _make_event(), _make_runner(), test_no_session_db(), test_set_title(), test_show_title_when_not_set(), test_show_title_when_set(), test_title_conflict(), test_title_control_chars_sanitized() (+4 more)

### Community 327 - "test_resume_command.py / _make_event()"
Cohesion: 0.4
Nodes (12): _make_event(), _make_runner(), _session_key_for_event(), test_list_named_sessions_when_no_arg(), test_list_shows_usage_when_no_titled(), test_no_session_db(), test_resume_already_on_session(), test_resume_auto_lineage() (+4 more)

### Community 328 - "test_managed_media_gatewa / _install_fake_tools_packa"
Cohesion: 0.41
Nodes (9): _install_fake_fal_client(), _install_fake_openai_module(), _install_fake_tools_package(), _load_tool_module(), test_managed_fal_submit_reuses_cached_sync_client(), test_managed_fal_submit_uses_gateway_origin_and_nous_token(), test_openai_tts_accepts_openai_api_key_as_direct_fallback(), test_openai_tts_uses_managed_audio_gateway_when_direct_key_absent() (+1 more)

### Community 329 - "test_cmd_update.py / _make_run_side_effect()"
Cohesion: 0.23
Nodes (9): _make_run_side_effect(), Tests for cmd_update — branch fallback when remote branch doesn't exist., When stdin/stdout aren't TTYs, config migration prompt is skipped., Build a side_effect function for subprocess.run that simulates git commands., cmd_update falls back to main when current branch has no remote counterpart., test_update_already_up_to_date(), test_update_falls_back_to_main_when_branch_not_on_remote(), test_update_uses_current_branch_when_on_remote() (+1 more)

### Community 330 - "test_skills_install_flags / test_cli_skills_install_f"
Cohesion: 0.17
Nodes (11): Tests for --yes / --force flag separation in `hermes skills install`.  --yes / -, Without flags, both force and yes should be False., --yes should set skip_confirm=True but NOT force., -y should behave the same as --yes., --force should set force=True but NOT yes., --force --yes should set both flags., test_cli_skills_install_force_and_yes_together(), test_cli_skills_install_force_sets_force() (+3 more)

### Community 331 - "TestOptionalEnvVarsRegist / .test_tavily_api_key_has_"
Cohesion: 0.17
Nodes (7): Verify that key env vars are registered in OPTIONAL_ENV_VARS., TAVILY_API_KEY is listed in OPTIONAL_ENV_VARS., TAVILY_API_KEY is in the 'tool' category., TAVILY_API_KEY is marked as password., TAVILY_API_KEY has a URL., TAVILY_API_KEY is listed in ENV_VARS_BY_VERSION., TestOptionalEnvVarsRegistry

### Community 332 - "test_banner_skills.py / test_get_available_skills"
Cohesion: 0.17
Nodes (11): Tests for banner get_available_skills() — disabled and platform filtering., get_available_skills should call _find_all_skills (which handles filtering)., Disabled skills should not appear in the banner count., No skills installed returns empty dict., If _find_all_skills import fails, return empty dict gracefully., Skills with None category should be grouped under 'general'., test_get_available_skills_delegates_to_find_all_skills(), test_get_available_skills_empty_when_no_skills() (+3 more)

### Community 333 - "_DummyCLI / test_cli_preloaded_skills"
Cohesion: 0.21
Nodes (5): _DummyCLI, _make_real_cli(), show_banner() no longer prints the activated skills line — it moved to run()., test_main_raises_for_unknown_preloaded_skill(), test_show_banner_does_not_print_skills()

### Community 334 - "_setup_callback() / TestApprovalMapping"
Cohesion: 0.23
Nodes (7): _make_response(), Tests for acp_adapter.permissions — ACP approval bridging., Helper to build a RequestPermissionResponse with the given outcome., Create a callback wired to a mock request_permission coroutine     that resolves, When the future times out, the callback should return 'deny'., _setup_callback(), TestApprovalMapping

### Community 335 - "FakeBot / FakeTree"
Cohesion: 0.2
Nodes (3): FakeBot, FakeTree, test_connect_releases_token_lock_on_timeout()

### Community 336 - "test_unauthorized_dm_beha / _clear_auth_env()"
Cohesion: 0.48
Nodes (11): _clear_auth_env(), _make_event(), _make_runner(), test_global_ignore_suppresses_pairing_reply(), test_rate_limited_user_gets_no_response(), test_rejection_message_records_rate_limit(), test_star_wildcard_in_allowlist_authorizes_any_user(), test_star_wildcard_works_for_any_platform() (+3 more)

### Community 337 - "test_session_race_guard.p / _make_runner()"
Cohesion: 0.41
Nodes (11): _make_event(), _make_runner(), test_command_messages_do_not_leave_sentinel(), test_second_message_during_sentinel_queued_not_duplicate(), test_sentinel_cleaned_up_after_handler_returns(), test_sentinel_cleaned_up_on_exception(), test_sentinel_placed_before_agent_setup(), test_shutdown_skips_sentinel() (+3 more)

### Community 338 - "simplify_redlines.py / _merge_tracked_changes_in"
Cohesion: 0.29
Nodes (11): _can_merge_tracked(), _find_elements(), _get_author(), _get_authors_from_docx(), get_tracked_change_authors(), infer_author(), _is_element(), _merge_tracked_changes_in() (+3 more)

### Community 339 - "ACP Editor Integration / MCP (Model Context Protoc"
Cohesion: 0.17
Nodes (12): Editor setup, Installation, Launching the ACP server, Registry manifest, What Hermes exposes in ACP mode, ACP Editor Integration, MCP (Model Context Protocol), Basic configuration reference (+4 more)

### Community 340 - "canvas_api.py / _paginated_get()"
Cohesion: 0.27
Nodes (9): _check_config(), _headers(), list_assignments(), list_courses(), _paginated_get(), Validate required environment variables are set., Fetch all pages up to max_items, following Canvas Link headers., List enrolled courses. (+1 more)

### Community 341 - "test_terminal_tool.py / Regression tests for sudo"
Cohesion: 0.18
Nodes (1): Regression tests for sudo detection and sudo password handling.

### Community 342 - "test_terminal_disk_usage. / TestDiskUsageGlob"
Cohesion: 0.18
Nodes (7): fake_scratch(), Tests for get_active_environments_info disk usage calculation., Create fake hermes scratch directories with known sizes., Each task should only count its own directories, not all hermes-* dirs., With 2 active tasks, each should count only its own dirs., TestDiskUsageGlob, TestDiskUsageWarningHardening

### Community 343 - "_make_cli() / test_cli_extension_hooks."
Cohesion: 0.27
Nodes (5): _make_cli(), Tests for protected HermesCLI TUI extension hooks.  Verifies that wrapper CLIs c, Create a HermesCLI with prompt_toolkit stubs (same pattern as test_cli_init)., TestExtensionHookDefaults, TestExtensionHookSubclass

### Community 344 - "_force_remove_worktree() / TestWorktreeIncludeSecuri"
Cohesion: 0.27
Nodes (5): _force_remove_worktree(), git_repo(), Security-focused integration tests for CLI worktree setup., Create a temporary git repo for testing real cli._setup_worktree behavior., TestWorktreeIncludeSecurity

### Community 345 - "TestDetectProvider / TestHasProvider"
Cohesion: 0.18
Nodes (3): Tests for acp_adapter.auth — provider detection., TestDetectProvider, TestHasProvider

### Community 346 - "TestDynamicRouteLoading / _make_adapter()"
Cohesion: 0.29
Nodes (3): _make_adapter(), Tests for webhook adapter dynamic route loading., TestDynamicRouteLoading

### Community 347 - "test_update_streaming.py / _make_runner()"
Cohesion: 0.38
Nodes (10): _make_event(), _make_runner(), test_cleans_up_on_completion(), test_detects_and_forwards_prompt(), test_failure_exit_code(), test_falls_back_when_adapter_unavailable(), test_intercepts_response_when_prompt_pending(), test_normal_message_when_no_prompt_pending() (+2 more)

### Community 348 - "StubAdapter / test_gateway_shutdown.py"
Cohesion: 0.25
Nodes (4): _source(), StubAdapter, test_cancel_background_tasks_cancels_inflight_message_processing(), test_gateway_stop_interrupts_running_agents_and_cancels_adapter_tasks()

### Community 349 - "TestExtractMedia / .test_cleaned_content_tri"
Cohesion: 0.18
Nodes (1): TestExtractMedia

### Community 350 - "clean.py / clean_unused_files()"
Cohesion: 0.33
Nodes (10): clean_unused_files(), get_referenced_files(), get_slide_referenced_files(), get_slides_in_sldidlst(), Remove unreferenced files from an unpacked PPTX directory.  Usage: python clean., remove_orphaned_files(), remove_orphaned_rels_files(), remove_orphaned_slides() (+2 more)

### Community 351 - "Writing Implementation Pl / Subagent-Driven Developme"
Cohesion: 0.18
Nodes (11): Bite-Sized Task Granularity (2-5 min), Plan Mode, RED-GREEN-REFACTOR Cycle, Pre-Commit Code Verification, Root Cause Analysis, Static Security Scan, Subagent-Driven Development, Systematic Debugging (+3 more)

### Community 352 - "codex_models.py / get_codex_model_ids()"
Cohesion: 0.31
Nodes (9): _add_forward_compat_models(), _fetch_models_from_api(), get_codex_model_ids(), Codex model discovery from API, local cache, and config., Return available Codex model IDs, trying API first, then local sources., Add Clawdbot-style synthetic forward-compat Codex models.      If a newer Codex, Fetch available models from the Codex API. Returns visible models sorted by prio, _read_cache_models() (+1 more)

### Community 353 - "database_server.py / _connect()"
Cohesion: 0.31
Nodes (9): _connect(), describe_table(), list_tables(), query(), List user-defined SQLite tables., Describe columns for a SQLite table., Run a read-only SELECT query and return rows plus column names., _reject_mutation() (+1 more)

### Community 354 - "test_setup_model_selectio / mock_provider_registry()"
Cohesion: 0.2
Nodes (5): mock_provider_registry(), Tests for _setup_provider_model_selection and the zai/kimi/minimax branch.  Regr, Minimal PROVIDER_REGISTRY entries for tested providers., Verify _setup_provider_model_selection works for all providers     that previous, TestSetupProviderModelSelection

### Community 355 - "TestDiscordThreadPersiste / ._make_adapter()"
Cohesion: 0.33
Nodes (1): TestDiscordThreadPersistence

### Community 356 - "test_discord_reactions.py / _make_event()"
Cohesion: 0.31
Nodes (7): adapter(), _make_event(), test_process_message_background_adds_and_swaps_reactions(), test_reaction_helper_failures_do_not_break_message_flow(), test_reactions_disabled_via_env(), test_reactions_disabled_via_env_zero(), test_reactions_enabled_by_default()

### Community 357 - "TestTruncateMessage / ._adapter()"
Cohesion: 0.38
Nodes (1): TestTruncateMessage

### Community 358 - "test_telegram_group_gatin / _group_message()"
Cohesion: 0.44
Nodes (8): _group_message(), _make_adapter(), _mention_entity(), test_free_response_chats_bypass_mention_requirement(), test_group_messages_can_be_opened_via_config(), test_group_messages_can_require_direct_trigger_via_config(), test_invalid_regex_patterns_are_ignored(), test_regex_mention_patterns_allow_custom_wake_words()

### Community 359 - "find_nearby.py / find_nearby()"
Cohesion: 0.31
Nodes (9): find_nearby(), geocode(), haversine(), _http_get(), _http_post(), main(), Distance in meters between two coordinates., Convert address/city/zip to coordinates via Nominatim. (+1 more)

### Community 360 - "GGUF Quantization Format / Guidance Constrained Gene"
Cohesion: 0.24
Nodes (10): Constrained LLM Generation, GGUF Advanced Usage, GGUF Quantization Format, Guidance Production Examples, Guidance Framework, Guidance Constrained Generation, Model Inference and Optimization, llama.cpp Inference Engine (+2 more)

### Community 361 - "AudioCraft: Audio Generat / MusicGen - Text-to-Music"
Cohesion: 0.22
Nodes (10): Audio Generation Techniques, AudioCraft Advanced Usage Guide, AudioGen - Text-to-Sound Effects, EnCodec - Neural Audio Codec, Melody Conditioning with Chroma, MusicGen - Text-to-Music, AudioCraft: Audio Generation (SKILL.md), Style-Conditioned Music Generation (+2 more)

### Community 362 - "Stable Diffusion Image Ge / Stable Diffusion Advanced"
Cohesion: 0.22
Nodes (10): CUDA Memory Optimization, HuggingFace Diffusers Library, Image Generation Techniques, Stable Diffusion Advanced Usage, ControlNet Spatial Conditioning, Inpainting - Masked Region Filling, LoRA Adapters for Fine-tuning, Stable Diffusion Image Generation (SKILL.md) (+2 more)

### Community 363 - "api_wrapper.py / _request()"
Cohesion: 0.33
Nodes (8): get_resource(), _headers(), health_check(), Check whether the upstream API is reachable., Fetch one resource by ID from the upstream API., Search upstream resources by query string., _request(), search_resources()

### Community 364 - "TestFindDocker / test_docker_find.py"
Cohesion: 0.22
Nodes (4): Tests for tools.environments.docker.find_docker — Docker CLI discovery., Clear the module-level docker executable cache between tests., _reset_cache(), TestFindDocker

### Community 365 - "test_modal_snapshot_isola / _install_modal_test_modul"
Cohesion: 0.5
Nodes (8): _install_modal_test_modules(), _load_module(), _reset_modules(), _restore_tool_modules(), test_modal_environment_cleanup_writes_namespaced_snapshot_key(), test_modal_environment_migrates_legacy_snapshot_key_and_uses_snapshot_id(), test_modal_environment_prunes_stale_direct_snapshot_and_retries_base_image(), test_resolve_modal_image_uses_snapshot_ids_and_registry_images()

### Community 366 - "TestEnsureLingerEnabled / test_gateway_linger.py"
Cohesion: 0.22
Nodes (2): Tests for gateway linger auto-enable behavior on headless Linux installs., TestEnsureLingerEnabled

### Community 367 - "test_nous_subscription.py / test_get_nous_subscriptio"
Cohesion: 0.22
Nodes (3): Tests for Nous subscription feature detection., When direct Browserbase keys are set and no managed gateway is available,     th, test_get_nous_subscription_features_uses_direct_browserbase_when_no_managed_gateway()

### Community 368 - "test_dict_tool_call_args. / _FakeChatCompletions"
Cohesion: 0.33
Nodes (5): _FakeChatCompletions, _FakeClient, _response_with_tool_call(), test_tool_call_validation_accepts_dict_arguments(), _tool_call()

### Community 369 - "test_telephony_skill.py / load_module()"
Cohesion: 0.42
Nodes (8): load_module(), test_diagnose_includes_decision_tree_and_saved_state(), test_messages_after_checkpoint_returns_only_newer_items(), test_save_twilio_writes_env_and_state(), test_twilio_buy_number_saves_env_and_state(), test_twilio_inbox_marks_seen_checkpoint(), test_upsert_env_updates_existing_values(), test_vapi_import_twilio_number_saves_phone_number_id()

### Community 370 - "test_telegram_conflict.py / _no_auto_discovery()"
Cohesion: 0.22
Nodes (3): _no_auto_discovery(), test_polling_conflict_becomes_fatal_after_retries(), test_polling_conflict_retries_before_fatal()

### Community 371 - "_would_warn() / TestAllowlistStartupCheck"
Cohesion: 0.33
Nodes (4): Tests for the startup allowlist warning check in gateway/run.py., Replicate the startup allowlist warning logic. Returns True if warning fires., TestAllowlistStartupCheck, _would_warn()

### Community 372 - "bridge.js / buildLidMap()"
Cohesion: 0.22
Nodes (0): 

### Community 373 - "add_slide.py / create_slide_from_layout("
Cohesion: 0.44
Nodes (7): _add_to_content_types(), _add_to_presentation_rels(), create_slide_from_layout(), duplicate_slide(), _get_next_slide_id(), get_next_slide_number(), Add a new slide to an unpacked PPTX directory.  Usage: python add_slide.py <unpa

### Community 374 - "gws_bridge.py / get_valid_token()"
Cohesion: 0.36
Nodes (8): get_hermes_home(), get_token_path(), get_valid_token(), main(), Refresh the access token using the refresh token., Return a valid access token, refreshing if needed., Refresh token if needed, then exec gws with remaining args., refresh_token()

### Community 375 - "neuroskill-bci / BCI"
Cohesion: 0.22
Nodes (9): BCI, biometrics, cognitive-state, EEG, focus, health, neurofeedback, neuroskill-bci (+1 more)

### Community 376 - "file_processor.py / _read_text()"
Cohesion: 0.36
Nodes (7): Return basic metadata and a preview for a UTF-8 text file., Find matching lines in a UTF-8 text file., Expose a text file as a resource., read_file_resource(), _read_text(), search_text_file(), summarize_text_file()

### Community 377 - "TestSaveConfigAtomicity / .test_atomic_write_create"
Cohesion: 0.25
Nodes (5): Verify save_config uses atomic writes (tempfile + os.replace)., If save_config crashes mid-write, the previous file stays intact., Failed writes must clean up their temp files., The written file must be valid YAML matching the input., TestSaveConfigAtomicity

### Community 378 - "test_batch_runner.py / cleanup_test_run()"
Cohesion: 0.32
Nodes (7): cleanup_test_run(), create_test_dataset(), main(), Create a small test dataset., Clean up test run output., Verify that output files were created correctly., verify_output()

### Community 379 - "test_terminalbench2_env_s / _load_terminalbench_modul"
Cohesion: 0.5
Nodes (7): _build_tar_b64(), _load_terminalbench_module(), Security tests for Terminal-Bench 2 archive extraction., _stub_module(), test_extract_base64_tar_allows_safe_files(), test_extract_base64_tar_rejects_path_traversal(), test_extract_base64_tar_rejects_symlinks()

### Community 380 - "TestCronJobCleanup / test_exit_cleanup_interru"
Cohesion: 0.25
Nodes (5): Tests for KeyboardInterrupt handling in exit cleanup paths.  ``except Exception`, cron/scheduler.py — end_session + close in the finally block., If end_session raises KeyboardInterrupt, close() must still run., If close() raises KeyboardInterrupt, it must not escape run_job., TestCronJobCleanup

### Community 381 - "test_telegram_text_batchi / _make_adapter()"
Cohesion: 0.61
Nodes (7): _make_adapter(), _make_event(), test_batch_cleans_up_after_flush(), test_different_chats_not_merged(), test_single_message_dispatched_after_delay(), test_split_messages_aggregated(), test_three_way_split_aggregated()

### Community 382 - "_load_ensure_ssl() / TestEnsureSslCerts"
Cohesion: 0.36
Nodes (4): _load_ensure_ssl(), Tests for SSL certificate auto-detection in gateway/run.py., Import _ensure_ssl_certs fresh (gateway/run.py has heavy deps, so we     extract, TestEnsureSslCerts

### Community 383 - "test_webhook_integration. / _create_app()"
Cohesion: 0.57
Nodes (7): _create_app(), _github_signature(), _make_adapter(), test_cross_platform_delivery(), test_github_comment_delivery(), test_github_pr_webhook_triggers_agent(), test_skills_injected_into_prompt()

### Community 384 - "test_status_command.py / _make_source()"
Cohesion: 0.64
Nodes (7): _make_event(), _make_runner(), _make_source(), test_handle_message_persists_agent_token_counts(), test_status_command_bypasses_active_session_guard(), test_status_command_includes_session_title_when_present(), test_status_command_reports_running_agent_without_interrupt()

### Community 385 - "test_verbose_command.py / _make_event()"
Cohesion: 0.61
Nodes (7): _make_event(), _make_runner(), test_cycles_through_all_modes(), test_defaults_to_all_when_no_tool_progress_set(), test_disabled_by_default(), test_enabled_cycles_mode(), test_no_config_file_returns_disabled()

### Community 386 - "test_unknown_command.py / _make_event()"
Cohesion: 0.64
Nodes (7): _make_event(), _make_runner(), _make_source(), test_known_slash_command_not_flagged_as_unknown(), test_underscored_alias_for_hyphenated_builtin_not_flagged(), test_unknown_slash_command_returns_guidance(), test_unknown_slash_command_underscored_form_also_guarded()

### Community 387 - "trajectory.py / convert_scratchpad_to_thi"
Cohesion: 0.25
Nodes (7): convert_scratchpad_to_think(), has_incomplete_scratchpad(), Trajectory saving utilities and static helpers.  _convert_to_trajectory_format s, Convert <REASONING_SCRATCHPAD> tags to <think> tags., Check if content has an opening <REASONING_SCRATCHPAD> without a closing tag., Append a trajectory entry to a JSONL file.      Args:         trajectory: The Sh, save_trajectory()

### Community 388 - "fetch_transcript.py / main()"
Cohesion: 0.36
Nodes (7): extract_video_id(), fetch_transcript(), format_timestamp(), main(), Extract the 11-character video ID from various YouTube URL formats., Convert seconds to HH:MM:SS or MM:SS format., Fetch transcript segments from YouTube.      Returns a list of dicts with 'text'

### Community 389 - "5-Minute Paper Explainer  / Manim Animation Framework"
Cohesion: 0.25
Nodes (8): Manim Animation Framework, Animation Easing Functions, p5.js Export Formats, p5.js Skill, 5-Minute Paper Explainer Template, Progressive Architecture Diagram Building, Equation Reveal Strategy, Narration-First Workflow

### Community 390 - "TestResolveCdpOverride / test_browser_cdp_override"
Cohesion: 0.29
Nodes (1): TestResolveCdpOverride

### Community 391 - "test_setup_matrix_e2ee.py / _parse_setup_imports()"
Cohesion: 0.33
Nodes (5): _parse_setup_imports(), Test that setup.py has shutil available for Matrix E2EE auto-install., shutil must be imported at module level so setup_gateway can use it         for, Parse setup.py and return top-level import names., TestSetupShutilImport

### Community 392 - "test_sessions_delete.py / test_sessions_delete_hand"
Cohesion: 0.29
Nodes (4): sessions delete should not crash when stdin is closed (non-TTY)., sessions prune should not crash when stdin is closed (non-TTY)., test_sessions_delete_handles_eoferror_on_confirm(), test_sessions_prune_handles_eoferror_on_confirm()

### Community 393 - "TestCronCommandLifecycle / test_cron.py"
Cohesion: 0.29
Nodes (2): Tests for hermes_cli.cron command handling., TestCronCommandLifecycle

### Community 394 - "TestAnthropicTokenMigrati / .test_clears_token_on_upg"
Cohesion: 0.38
Nodes (4): Test that config version 8→9 clears ANTHROPIC_TOKEN., ANTHROPIC_TOKEN is cleared unconditionally when upgrading to v9., Already at v9 — ANTHROPIC_TOKEN is not touched., TestAnthropicTokenMigration

### Community 395 - "test_auth_nous_provider.p / _setup_nous_auth()"
Cohesion: 0.43
Nodes (5): Regression tests for Nous OAuth refresh + agent-key mint interactions., _setup_nous_auth(), test_mint_retry_uses_latest_rotated_refresh_token(), test_refresh_token_persisted_when_mint_returns_insufficient_credits(), test_refresh_token_persisted_when_mint_times_out()

### Community 396 - "test_usage_pricing.py / test_custom_endpoint_mode"
Cohesion: 0.29
Nodes (0): 

### Community 397 - "test_smart_model_routing. / test_resolve_turn_route_f"
Cohesion: 0.29
Nodes (0): 

### Community 398 - "test_session_model_reset. / _make_source()"
Cohesion: 0.81
Nodes (6): _make_event(), _make_runner(), _make_source(), test_new_command_clears_session_model_override(), test_new_command_no_override_is_noop(), test_new_command_only_clears_own_session()

### Community 399 - "redact.py / redact_sensitive_text()"
Cohesion: 0.33
Nodes (5): _mask_token(), Regex-based secret redaction for logs and tool output.  Applies pattern matching, Mask a token, preserving prefix for long tokens., Apply all redaction patterns to a block of text.      Safe to call on any string, redact_sensitive_text()

### Community 400 - "Hermes Honcho Integration / Async Prefetch Pattern"
Cohesion: 0.29
Nodes (7): AI Peer Identity Formation, Async Prefetch Pattern, Context Injection Latency Problem, Dual Peer Model, Hermes Honcho Integration, Honcho Integration Specification, Per-Peer Memory Modes

### Community 401 - "gitnexus-explorer / parallel-cli"
Cohesion: 0.52
Nodes (7): bioinformatics, domain-intel, duckduckgo-search, gitnexus-explorer, parallel-cli, qmd, scrapling

### Community 402 - "Linear Design System / Stripe Design System"
Cohesion: 0.33
Nodes (7): Font Substitution Reference, Linear Color Palette, Linear Design System, Linear Typography (Inter Variable), Stripe Color Palette, Stripe Design System, Stripe Typography (sohne-var)

### Community 403 - "Hermes Agent Banner / Arcade Gaming Theme"
Cohesion: 0.33
Nodes (7): Arcade Gaming Theme, Hermes Agent Banner, HERMES-AGENT Text, Yellow-Bronze Color Scheme, Dark Background, Outlined Letter Effect, Retro Pixel Art Aesthetic

### Community 404 - "Caduceus Icon / Gold Gradient"
Cohesion: 0.48
Nodes (7): Caduceus Icon, Central Staff, Gold Gradient, Left Serpent, Orb at Top, Right Serpent, Wings

### Community 405 - "url_safety.py / _is_blocked_ip()"
Cohesion: 0.4
Nodes (5): _is_blocked_ip(), is_safe_url(), URL safety checks — blocks requests to private/internal network addresses.  Prev, Return True if the IP should be blocked for SSRF protection., Return True if the URL target is not a private/internal address.      Resolves t

### Community 406 - "openrouter_client.py / check_api_key()"
Cohesion: 0.33
Nodes (5): check_api_key(), get_async_client(), Shared OpenRouter API client for Hermes tools.  Provides a single lazy-initializ, Return a shared async OpenAI-compatible client for OpenRouter.      The client i, Check whether the OpenRouter API key is present.

### Community 407 - "colors.py / color()"
Cohesion: 0.4
Nodes (5): color(), Shared ANSI color utilities for Hermes CLI modules., Apply color codes to text (only when color output is appropriate)., Return True when colored output is appropriate.      Respects the NO_COLOR envir, should_use_color()

### Community 408 - "extract-skills.py / main()"
Cohesion: 0.6
Nodes (5): _consolidate_small_categories(), extract_cached_index_skills(), extract_local_skills(), _guess_category(), main()

### Community 409 - "test_managed_tool_gateway / test_read_nous_access_tok"
Cohesion: 0.33
Nodes (0): 

### Community 410 - "test_subprocess_timeouts. / _subprocess_run_calls()"
Cohesion: 0.4
Nodes (5): Tests for subprocess.run() timeout coverage in CLI utilities., Parse a Python file and return info about subprocess.run() calls., Every subprocess.run() call in CLI modules must specify a timeout., _subprocess_run_calls(), test_all_subprocess_run_calls_have_timeout()

### Community 411 - "test_placeholder_usage.py / Tests for CLI placeholder"
Cohesion: 0.33
Nodes (1): Tests for CLI placeholder text in config/setup output.

### Community 412 - "test_managed_installs.py / test_cmd_update_blocks_ma"
Cohesion: 0.33
Nodes (0): 

### Community 413 - "TestRemoveEnvValue / .test_clears_os_environ()"
Cohesion: 0.33
Nodes (1): TestRemoveEnvValue

### Community 414 - "test_plan_command.py / test_plan_command_appears"
Cohesion: 0.73
Nodes (5): _make_event(), _make_plan_skill(), _make_runner(), test_plan_command_appears_in_help_output_via_skill_listing(), test_plan_command_loads_skill_and_runs_agent()

### Community 415 - "prompt_caching.py / apply_anthropic_cache_con"
Cohesion: 0.4
Nodes (5): apply_anthropic_cache_control(), _apply_cache_marker(), Anthropic prompt caching (system_and_3 strategy).  Reduces input token costs by, Add cache_control to a single message, handling all format variations., Apply system_and_3 caching strategy to messages for Anthropic models.      Place

### Community 416 - "allowlist.js / expandWhatsAppIdentifiers"
Cohesion: 0.6
Nodes (4): expandWhatsAppIdentifiers(), matchesAllowedUser(), normalizeWhatsAppIdentifier(), readMappingFile()

### Community 417 - "upload() / upload.py"
Cohesion: 0.47
Nodes (5): concat_buffers(), main(), Build the Excalidraw v2 concat-buffers binary format.      Layout: [version=1 (4, Encrypt and upload Excalidraw JSON to excalidraw.com.      Args:         excalid, upload()

### Community 418 - "extract_pymupdf.py / extract_images()"
Cohesion: 0.33
Nodes (0): 

### Community 419 - "RAG Applications / FAISS Similarity Search"
Cohesion: 0.33
Nodes (6): Chroma Vector Database, FAISS Similarity Search, Instructor Structured Output, RAG Applications, Structured Output Extraction, Vector Search

### Community 420 - "Docker / Environment variable forw"
Cohesion: 0.33
Nodes (6): Docker, Environment variable forwarding, Persistent volumes, Quick start, Running in gateway mode, Running interactively (CLI chat)

### Community 421 - "Git Worktrees / Best Practices"
Cohesion: 0.33
Nodes (6): Git Worktrees, Best Practices, Cleaning Up Worktrees Safely, Quick Start: Creating a Worktree, Running Multiple Agents in Parallel, Why Use Worktrees with Hermes?

### Community 422 - "Batch Processing / Configuration Options"
Cohesion: 0.33
Nodes (6): Configuration Options, Dataset Format, Overview, Quick Start, Toolset Distributions, Batch Processing

### Community 423 - "Skins & Themes / Built-in skins"
Cohesion: 0.33
Nodes (6): Skins & Themes, Built-in skins, Change skins, Complete list of configurable keys, Custom skins, Hermes Mod — Visual Skin Editor

### Community 424 - "Personality & SOUL.md / Good SOUL.md content"
Cohesion: 0.33
Nodes (6): Personality & SOUL.md, Good SOUL.md content, How SOUL.md works now, What should go in SOUL.md?, Where to edit it, Why this design

### Community 425 - "Fallback-Providers / Auxiliary Task Fallback"
Cohesion: 0.33
Nodes (6): Fallback-Providers, Auxiliary Task Fallback, Context Compression Fallback, Cron Job Providers, Delegation Provider Override, Primary Model Fallback

### Community 426 - "clarify_tool.py / check_clarify_requirement"
Cohesion: 0.4
Nodes (4): check_clarify_requirements(), clarify_tool(), Ask the user a question, optionally with multiple-choice options.      Args:, Clarify tool has no external requirements -- always available.

### Community 427 - "env_loader.py / load_hermes_dotenv()"
Cohesion: 0.5
Nodes (4): _load_dotenv_with_fallback(), load_hermes_dotenv(), Helpers for loading Hermes .env files consistently across entrypoints., Load Hermes environment files with user config taking precedence.      Behavior:

### Community 428 - "test_project_metadata.py / test_matrix_extra_exists_"
Cohesion: 0.5
Nodes (4): _load_optional_dependencies(), Regression tests for packaging metadata in pyproject.toml., matrix-nio[e2e] depends on python-olm which is upstream-broken on modern     mac, test_matrix_extra_exists_but_excluded_from_all()

### Community 429 - "test_mcp_tool_issue_948.p / test_format_connect_error"
Cohesion: 0.4
Nodes (0): 

### Community 430 - "test_env_loader.py / test_main_import_applies_"
Cohesion: 0.4
Nodes (0): 

### Community 431 - "_FakeTerminalMenu / test_reasoning_effort_men"
Cohesion: 0.4
Nodes (1): _FakeTerminalMenu

### Community 432 - "test_banner_git_state.py / test_format_banner_versio"
Cohesion: 0.4
Nodes (0): 

### Community 433 - "test_chat_skills_flag.py / test_chat_subcommand_acce"
Cohesion: 0.4
Nodes (0): 

### Community 434 - "TestSaveEnvValueSecure / .test_save_env_value_hard"
Cohesion: 0.4
Nodes (1): TestSaveEnvValueSecure

### Community 435 - "test_anthropic_provider_p / Tests for Anthropic crede"
Cohesion: 0.4
Nodes (1): Tests for Anthropic credential persistence helpers.

### Community 436 - "test_stt_config.py / test_enrich_message_with_"
Cohesion: 0.4
Nodes (0): 

### Community 437 - "pack.py / pack()"
Cohesion: 0.6
Nodes (4): _condense_xml(), pack(), Pack a directory into a DOCX, PPTX, or XLSX file.  Validates with auto-repair, c, _run_validation()

### Community 438 - "GitHub Authentication Set / GitHub Code Review Skill"
Cohesion: 0.4
Nodes (5): Structured Code Review Process, GitHub CLI Tool, Git HTTPS and SSH Authentication, GitHub Authentication Setup Skill, GitHub Code Review Skill

### Community 439 - "Songsee Audio Visualizati / Media Skills Collection"
Cohesion: 0.4
Nodes (5): Audio Feature Visualization, Audio Feature Visualization, Media Skills Collection, Midjourney Image Generation Skill, Songsee Audio Visualization

### Community 440 - "Polymarket API Endpoints / Polymarket Prediction Mar"
Cohesion: 0.4
Nodes (5): Polymarket API Endpoints, CLOB API - Real-time Prices, Gamma API - Discovery & Search, Polymarket Market Structure, Polymarket Prediction Market Skill

### Community 441 - "Subagent Delegation Patte / Code Review Delegation Pa"
Cohesion: 0.4
Nodes (5): Code Review Delegation Pattern, Subagent Delegation Feature, Subagent Delegation Patterns, Multi-File Parallel Refactoring, Parallel Research Workflow

### Community 442 - "Discord Messaging Platfor / Slack Messaging Platform"
Cohesion: 0.6
Nodes (5): Discord Messaging Platform, Mattermost Messaging Platform, Slack Messaging Platform, Telegram Messaging Platform, Voice & Text-to-Speech

### Community 443 - "Home Assistant Platform / Smart Device Control"
Cohesion: 0.5
Nodes (5): Smart Device Control, Home Assistant Tools (4 LLM-callable tools), Home Assistant WebSocket, Home Assistant Platform, Blocked Service Domains

### Community 444 - "Hermes Response Messages / Previous Conversation Hea"
Cohesion: 0.4
Nodes (5): Hermes Response Messages, Previous Conversation Header, Session Recap Panel, Tool Calls Summary, User Query Messages

### Community 445 - "ansi_strip.py / strip_ansi()"
Cohesion: 0.5
Nodes (3): Strip ANSI escape sequences from subprocess output.  Used by terminal_tool, code, Remove ANSI escape sequences from text.      Returns the input unchanged (fast p, strip_ansi()

### Community 446 - "_write_wav() / neutts_synth.py"
Cohesion: 0.67
Nodes (3): main(), Write a WAV file from float32 samples (no soundfile dependency)., _write_wav()

### Community 447 - "binary_extensions.py / has_binary_extension()"
Cohesion: 0.5
Nodes (3): has_binary_extension(), Binary file extensions to skip for text-based operations.  These files can't be, Check if a file path has a binary extension. Pure string check, no I/O.

### Community 448 - "scaffold_fastmcp.py / list_templates()"
Cohesion: 1.0
Nodes (3): list_templates(), main(), render_template()

### Community 449 - "patches.py / apply_patches()"
Cohesion: 0.5
Nodes (3): apply_patches(), Monkey patches for making hermes-agent tools work inside async frameworks (Atrop, Apply all monkey patches needed for Atropos compatibility.

### Community 450 - "test_terminal_none_comman / Regression tests for inva"
Cohesion: 0.5
Nodes (1): Regression tests for invalid/None terminal command handling.

### Community 451 - "test_mixture_of_agents_to / test_moa_defaults_track_c"
Cohesion: 0.5
Nodes (0): 

### Community 452 - "test_skills_subparser.py / test_no_duplicate_skills_"
Cohesion: 0.5
Nodes (3): Test that skills subparser doesn't conflict (regression test for #898)., Ensure 'skills' subparser is only registered once to avoid Python 3.11+ crash., test_no_duplicate_skills_subparser()

### Community 453 - "test_anthropic_oauth_flow / Tests for Anthropic OAuth"
Cohesion: 0.5
Nodes (1): Tests for Anthropic OAuth setup flow behavior.

### Community 454 - "TestEnsureHermesHome / .test_creates_default_sou"
Cohesion: 0.5
Nodes (1): TestEnsureHermesHome

### Community 455 - "TestSaveAndLoadRoundtrip / .test_nested_values_prese"
Cohesion: 0.5
Nodes (1): TestSaveAndLoadRoundtrip

### Community 456 - "test_setup_prompt_menus.p / test_prompt_checklist_use"
Cohesion: 0.5
Nodes (0): 

### Community 457 - "test_launcher.py / test_launcher_delegates_t"
Cohesion: 0.5
Nodes (3): Tests for the top-level `./hermes` launcher script., `./hermes` should use `hermes_cli.main`, not the legacy Fire wrapper., test_launcher_delegates_to_argparse_entrypoint()

### Community 458 - "test_cli_retry.py / Regression tests for CLI "
Cohesion: 0.5
Nodes (1): Regression tests for CLI /retry history replacement semantics.

### Community 459 - "test_discord_imports.py / TestDiscordImportSafety"
Cohesion: 0.5
Nodes (2): Import-safety tests for the Discord gateway adapter., TestDiscordImportSafety

### Community 460 - "permissions.py / make_approval_callback()"
Cohesion: 0.5
Nodes (3): make_approval_callback(), ACP permission bridging — maps ACP approval requests to hermes approval callback, Return a hermes-compatible ``approval_callback(command, description) -> str``

### Community 461 - "extract_marker.py / check_requirements()"
Cohesion: 0.5
Nodes (2): check_requirements(), Check disk space before installing.

### Community 462 - ".discover_and_load() / ._register_builtin_hooks("
Cohesion: 0.5
Nodes (2): Register built-in hooks that are always active., Scan the hooks directory for hook directories and load their handlers.

### Community 463 - "Pricing Accuracy Architec / Usage Normalization"
Cohesion: 0.5
Nodes (4): Cache-Aware Billing, Canonical Usage Record, Pricing Accuracy Architecture, Usage Normalization

### Community 464 - "Attention Optimization / Distributed Training"
Cohesion: 0.5
Nodes (4): HuggingFace Accelerate, Attention Optimization, Distributed Training, Flash Attention

### Community 465 - "add_updater Pattern / ValueTracker"
Cohesion: 0.5
Nodes (4): add_updater Pattern, always_redraw, DecimalNumber, ValueTracker

### Community 466 - "ElevenLabs Design System / Luma Design System"
Cohesion: 1.0
Nodes (4): ElevenLabs Design System, Luma Design System, Midjourney Design System, Pika Design System

### Community 467 - "Xitter (X/Twitter) Skill / Social Media Skills"
Cohesion: 0.5
Nodes (4): Social Media Skills, X API Credentials, x-cli Terminal Client, Xitter (X/Twitter) Skill

### Community 468 - "llama.cpp Backend Runtime / Local LLM Setup on macOS"
Cohesion: 0.67
Nodes (4): llama.cpp Backend Runtime, Local LLM Setup on macOS, MLX/omlx Backend Runtime, OpenAI-Compatible API Endpoints

### Community 469 - "Model Context Protocol In / MCP Server Configuration "
Cohesion: 0.5
Nodes (4): Context Management & Compression, MCP Feature & Integration, Model Context Protocol Integration, MCP Server Configuration & Filtering

### Community 470 - "HermesAgent / hermes-agent.rb"
Cohesion: 0.67
Nodes (1): HermesAgent

### Community 471 - "test_packaging_metadata.p / test_faster_whisper_is_no"
Cohesion: 0.67
Nodes (0): 

### Community 472 - "test_setup_hermes_script. / test_setup_hermes_script_"
Cohesion: 0.67
Nodes (0): 

### Community 473 - "TestGetHermesHome / .test_default_path()"
Cohesion: 0.67
Nodes (1): TestGetHermesHome

### Community 474 - "TestLoadConfigDefaults / .test_legacy_root_level_m"
Cohesion: 0.67
Nodes (1): TestLoadConfigDefaults

### Community 475 - "test_entry.py / Tests for acp_adapter.ent"
Cohesion: 0.67
Nodes (1): Tests for acp_adapter.entry startup wiring.

### Community 476 - "test_retry_replacement.py / test_gateway_retry_replac"
Cohesion: 0.67
Nodes (0): 

### Community 477 - "test_telegram_photo_inter / _make_runner()"
Cohesion: 1.0
Nodes (2): _make_runner(), test_handle_message_does_not_priority_interrupt_photo_followup()

### Community 478 - "test_session_env.py / test_clear_session_env_re"
Cohesion: 0.67
Nodes (0): 

### Community 479 - "test_discord_send.py / _ensure_discord_mock()"
Cohesion: 0.67
Nodes (0): 

### Community 480 - "load_godmode.py / _gm_load()"
Cohesion: 0.67
Nodes (1): Loader for G0DM0D3 scripts. Handles the exec-scoping issues.  Usage in execute_c

### Community 481 - "export-frames.js / main()"
Cohesion: 1.0
Nodes (2): main(), parseArgs()

### Community 482 - "hooks.py / loaded_hooks()"
Cohesion: 0.67
Nodes (1): Event Hook System  A lightweight event-driven system that fires handlers at key

### Community 483 - "SimPO Training Workflow / Beta (Reward Scaling) Hyp"
Cohesion: 0.67
Nodes (3): Beta (Reward Scaling) Hyperparameter, DeepSpeed ZeRO-3 Integration, SimPO Training Workflow

### Community 484 - "YouTube Content Tool / Transcript Extraction and"
Cohesion: 0.67
Nodes (3): Transcript Extraction and Transformation, YouTube Content Tool, YouTube Output Formats

### Community 485 - "OpenHue Skill / IoT Automation"
Cohesion: 0.67
Nodes (3): IoT Automation, OpenHue Skill, Philips Hue Lights Control

### Community 486 - "SOUL.md - Agent Identity  / AGENTS.md - Project Conte"
Cohesion: 0.67
Nodes (3): AGENTS.md - Project Context, Personality & Mode Switching, SOUL.md - Agent Identity System

### Community 487 - "Tool Output Management / Image Generation"
Cohesion: 0.67
Nodes (3): Image Generation, Subagent Delegation, Tool Output Management

### Community 488 - "default_soul.py / Default SOUL.md template "
Cohesion: 1.0
Nodes (1): Default SOUL.md template seeded into HERMES_HOME on first run.

### Community 489 - "index.tsx / handler()"
Cohesion: 1.0
Nodes (0): 

### Community 490 - "test_gateway_runtime_heal / test_runtime_health_lines"
Cohesion: 1.0
Nodes (0): 

### Community 491 - "test_discord_media_metada / test_discord_media_method"
Cohesion: 1.0
Nodes (0): 

### Community 492 - "search_arxiv.py / search()"
Cohesion: 1.0
Nodes (0): 

### Community 493 - "MSE + L1 Sparsity Loss / SAE Training Workflow"
Cohesion: 1.0
Nodes (2): MSE + L1 Sparsity Loss, SAE Training Workflow

### Community 494 - "Figma Design System / Miro Design System"
Cohesion: 1.0
Nodes (2): Figma Design System, Miro Design System

### Community 495 - "Codebase Inspection Skill / Pygount Lines of Code Ana"
Cohesion: 1.0
Nodes (2): Codebase Inspection Skill, Pygount Lines of Code Analyzer

### Community 496 - "Fallback Providers / Honcho Cross-Session Memo"
Cohesion: 1.0
Nodes (2): Fallback Providers, Honcho Cross-Session Memory

### Community 497 - "Hermes Search / Session Recap"
Cohesion: 1.0
Nodes (2): Hermes Search, Session Recap

### Community 498 - "Signal Messaging Platform / WhatsApp Messaging Platfo"
Cohesion: 1.0
Nodes (2): Signal Messaging Platform, WhatsApp Messaging Platform

### Community 499 - "Home Assistant Messaging  / Open WebUI Messaging Plat"
Cohesion: 1.0
Nodes (2): Home Assistant Messaging Platform, Open WebUI Messaging Platform

### Community 500 - "Load configuration from Y"
Cohesion: 1.0
Nodes (1): Load configuration from YAML file.

### Community 501 - "Normalize summary-model o"
Cohesion: 1.0
Nodes (1): Normalize summary-model output to a safe string.

### Community 502 - "Normalize summary text to"
Cohesion: 1.0
Nodes (1): Normalize summary text to include the expected prefix exactly once.

### Community 503 - "Validate and sanitize a s"
Cohesion: 1.0
Nodes (1): Validate and sanitize a session title.          - Strips leading/trailing whites

### Community 504 - "Sanitize user input for s"
Cohesion: 1.0
Nodes (1): Sanitize user input for safe use in FTS5 MATCH queries.          FTS5 has its ow

### Community 505 - "Current audio input RMS l"
Cohesion: 1.0
Nodes (1): Current audio input RMS level (0-32767). Updated each audio chunk.

### Community 506 - "Write numpy int16 audio d"
Cohesion: 1.0
Nodes (1): Write numpy int16 audio data to a WAV file.          Returns the file path.

### Community 507 - "Strip shell startup warni"
Cohesion: 1.0
Nodes (1): Strip shell startup warnings from the beginning of output.

### Community 508 - "Best-effort liveness chec"
Cohesion: 1.0
Nodes (1): Best-effort liveness check for host-visible PIDs.

### Community 509 - "Terminate a host-visible "
Cohesion: 1.0
Nodes (1): Terminate a host-visible PID without requiring the original process handle.

### Community 510 - "Return the writable sandb"
Cohesion: 1.0
Nodes (1): Return the writable sandbox temp dir for env-backed background tasks.

### Community 511 - "Acquire an exclusive file"
Cohesion: 1.0
Nodes (1): Acquire an exclusive file lock for read-modify-write safety.          Uses a sep

### Community 512 - "Read a memory file and sp"
Cohesion: 1.0
Nodes (1): Read a memory file and split into entries.          No file locking needed: _wri

### Community 513 - "Write entries to a memory"
Cohesion: 1.0
Nodes (1): Write entries to a memory file using atomic temp-file + rename.          Previou

### Community 514 - "Extract text from a ToolR"
Cohesion: 1.0
Nodes (1): Extract text from a ToolResultContent block.

### Community 515 - "Return ErrorData (MCP spe"
Cohesion: 1.0
Nodes (1): Return ErrorData (MCP spec) or raise as fallback.

### Community 516 - "Validate and normalize a "
Cohesion: 1.0
Nodes (1): Validate and normalize a todo item.          Ensures required fields exist and s

### Community 517 - "Read a file with paginati"
Cohesion: 1.0
Nodes (1): Read a file with pagination support.

### Community 518 - "Write content to a file, "
Cohesion: 1.0
Nodes (1): Write content to a file, creating directories as needed.

### Community 519 - "Replace text in a file us"
Cohesion: 1.0
Nodes (1): Replace text in a file using fuzzy matching.

### Community 520 - "Apply a V4A format patch."
Cohesion: 1.0
Nodes (1): Apply a V4A format patch.

### Community 521 - "Search for content or fil"
Cohesion: 1.0
Nodes (1): Search for content or files.

### Community 522 - "Parse git --shortstat out"
Cohesion: 1.0
Nodes (1): Parse git --shortstat output into entry dict.

### Community 523 - "Short, human-readable nam"
Cohesion: 1.0
Nodes (1): Short, human-readable name shown in logs and diagnostics.

### Community 524 - "Return True when all requ"
Cohesion: 1.0
Nodes (1): Return True when all required env vars / credentials are present.          Calle

### Community 525 - "Create a cloud browser se"
Cohesion: 1.0
Nodes (1): Create a cloud browser session and return session metadata.          Must return

### Community 526 - "Release / terminate a clo"
Cohesion: 1.0
Nodes (1): Release / terminate a cloud session by its provider session ID.          Returns

### Community 527 - "Best-effort session teard"
Cohesion: 1.0
Nodes (1): Best-effort session teardown during process exit.          Called from atexit /

### Community 528 - "Release backend resources"
Cohesion: 1.0
Nodes (1): Release backend resources (container, instance, connection).

### Community 529 - "Append stdin_data as a sh"
Cohesion: 1.0
Nodes (1): Append stdin_data as a shell heredoc to the command string.

### Community 530 - "Return replacement text f"
Cohesion: 1.0
Nodes (1): Return replacement text for a completion.          When the user has already typ

### Community 531 - "Extract the current word "
Cohesion: 1.0
Nodes (1): Extract the current word if it looks like a file path.          Returns the path

### Community 532 - "Yield Completion objects "
Cohesion: 1.0
Nodes (1): Yield Completion objects for file paths matching *word*.

### Community 533 - "Extract a bare ``@`` toke"
Cohesion: 1.0
Nodes (1): Extract a bare ``@`` token for context reference completions.

### Community 534 - "Yield Claude Code-style @"
Cohesion: 1.0
Nodes (1): Yield Claude Code-style @ context completions.          Bare ``@`` or ``@partial

### Community 535 - "Create config from enviro"
Cohesion: 1.0
Nodes (1): Create config from environment variables (fallback).

### Community 536 - "Create config from the re"
Cohesion: 1.0
Nodes (1): Create config from the resolved Honcho config path.          Resolution: $HERMES

### Community 537 - "Return the git repo root "
Cohesion: 1.0
Nodes (1): Return the git repo root directory name, or None if not in a repo.

### Community 538 - "Get the Honcho client, in"
Cohesion: 1.0
Nodes (1): Get the Honcho client, initializing if needed.

### Community 539 - "Format local messages as "
Cohesion: 1.0
Nodes (1): Format local messages as an XML transcript for Honcho file upload.

### Community 540 - "Normalize Honcho card pay"
Cohesion: 1.0
Nodes (1): Normalize Honcho card payloads into a plain list of strings.

### Community 541 - "docusaurus.config.ts"
Cohesion: 1.0
Nodes (0): 

### Community 542 - "sidebars.ts"
Cohesion: 1.0
Nodes (0): 

### Community 543 - "_run_async should still w"
Cohesion: 1.0
Nodes (1): _run_async should still work when called from inside an         already-running

### Community 544 - "test_minisweagent_path.py"
Cohesion: 1.0
Nodes (0): 

### Community 545 - "Lazy-import execute_code "
Cohesion: 1.0
Nodes (1): Lazy-import execute_code to avoid pulling in firecrawl at collection time.

### Community 546 - "Read then write with no e"
Cohesion: 1.0
Nodes (1): Read then write with no external modification — no warning.

### Community 547 - "Read, then external modif"
Cohesion: 1.0
Nodes (1): Read, then external modify, then write — should warn.

### Community 548 - "Writing a file that was n"
Cohesion: 1.0
Nodes (1): Writing a file that was never read — no warning.

### Community 549 - "Creating a new file — no "
Cohesion: 1.0
Nodes (1): Creating a new file — no warning.

### Community 550 - "Task A reads, file change"
Cohesion: 1.0
Nodes (1): Task A reads, file changes, Task B writes — no warning for B.

### Community 551 - "Patch should warn if the "
Cohesion: 1.0
Nodes (1): Patch should warn if the target file changed since last read.

### Community 552 - "Patch with no external ch"
Cohesion: 1.0
Nodes (1): Patch with no external changes — no warning.

### Community 553 - "A read that returns >max "
Cohesion: 1.0
Nodes (1): A read that returns >max chars is rejected.

### Community 554 - "Normal-sized reads pass t"
Cohesion: 1.0
Nodes (1): Normal-sized reads pass through fine.

### Community 555 - "Content just under the li"
Cohesion: 1.0
Nodes (1): Content just under the limit should pass through fine.

### Community 556 - "Second read of same file+"
Cohesion: 1.0
Nodes (1): Second read of same file+range returns dedup stub.

### Community 557 - "After the file is modifie"
Cohesion: 1.0
Nodes (1): After the file is modified, dedup returns full content.

### Community 558 - "Same file but different o"
Cohesion: 1.0
Nodes (1): Same file but different offset/limit should not dedup.

### Community 559 - "Different task_ids have s"
Cohesion: 1.0
Nodes (1): Different task_ids have separate dedup caches.

### Community 560 - "After reset_file_dedup, t"
Cohesion: 1.0
Nodes (1): After reset_file_dedup, the same read returns full content.

### Community 561 - "reset_file_dedup(None) cl"
Cohesion: 1.0
Nodes (1): reset_file_dedup(None) clears all tasks.

### Community 562 - "reset_file_dedup does NOT"
Cohesion: 1.0
Nodes (1): reset_file_dedup does NOT affect the consecutive-read counter.

### Community 563 - "A config value of 50 shou"
Cohesion: 1.0
Nodes (1): A config value of 50 should reject reads over 50 chars.

### Community 564 - "A config value of 500K sh"
Cohesion: 1.0
Nodes (1): A config value of 500K should allow reads up to 500K chars.

### Community 565 - "When tasks array is provi"
Cohesion: 1.0
Nodes (1): When tasks array is provided, top-level goal/context/toolsets are ignored.

### Community 566 - "When delegation.provider "
Cohesion: 1.0
Nodes (1): When delegation.provider is set, full credentials are resolved.

### Community 567 - "Nous provider resolves No"
Cohesion: 1.0
Nodes (1): Nous provider resolves Nous Portal base_url and api_key.

### Community 568 - "When provider resolution "
Cohesion: 1.0
Nodes (1): When provider resolution fails, ValueError is raised with helpful message.

### Community 569 - "When provider resolves bu"
Cohesion: 1.0
Nodes (1): When provider resolves but has no API key, ValueError is raised.

### Community 570 - "When delegation.provider "
Cohesion: 1.0
Nodes (1): When delegation.provider is configured, child agent gets resolved credentials.

### Community 571 - "Parent on Nous, subagent "
Cohesion: 1.0
Nodes (1): Parent on Nous, subagent on OpenRouter — full credential switch.

### Community 572 - "When delegation config is"
Cohesion: 1.0
Nodes (1): When delegation config is empty, child inherits parent credentials.

### Community 573 - "When credential resolutio"
Cohesion: 1.0
Nodes (1): When credential resolution fails, delegate_task returns a JSON error.

### Community 574 - "In batch mode, all childr"
Cohesion: 1.0
Nodes (1): In batch mode, all children receive the resolved credentials.

### Community 575 - "Setting only model (no pr"
Cohesion: 1.0
Nodes (1): Setting only model (no provider) changes model but keeps parent credentials.

### Community 576 - "Shared patches for pre-na"
Cohesion: 1.0
Nodes (1): Shared patches for pre-navigation tests that pass the SSRF check.

### Community 577 - "Shared patches for redire"
Cohesion: 1.0
Nodes (1): Shared patches for redirect tests.

### Community 578 - "On Windows, the old check"
Cohesion: 1.0
Nodes (1): On Windows, the old check incorrectly blocks valid subpaths.

### Community 579 - "tirith block goes through"
Cohesion: 1.0
Nodes (1): tirith block goes through approval flow (user gets prompted).

### Community 580 - "tirith block + dangerous "
Cohesion: 1.0
Nodes (1): tirith block + dangerous pattern → combined approval prompt.

### Community 581 - "In gateway mode, tirith b"
Cohesion: 1.0
Nodes (1): In gateway mode, tirith block should return approval_required.

### Community 582 - "Both tirith warn and dang"
Cohesion: 1.0
Nodes (1): Both tirith warn and dangerous → single approval_required with both keys.

### Community 583 - "Non-ImportError exception"
Cohesion: 1.0
Nodes (1): Non-ImportError exceptions from tirith wrapper should propagate.

### Community 584 - "After a failed download, "
Cohesion: 1.0
Nodes (1): After a failed download, subsequent resolves must not retry.

### Community 585 - "After cached miss, check_"
Cohesion: 1.0
Nodes (1): After cached miss, check_command_security hits OSError → fail_open.

### Community 586 - "An explicit tirith_path t"
Cohesion: 1.0
Nodes (1): An explicit tirith_path that doesn't exist must NOT trigger download.

### Community 587 - "An explicit ~/path that d"
Cohesion: 1.0
Nodes (1): An explicit ~/path that doesn't exist must NOT trigger download.

### Community 588 - "The default bare 'tirith'"
Cohesion: 1.0
Nodes (1): The default bare 'tirith' SHOULD trigger auto-download.

### Community 589 - "cosign verify-blob exits "
Cohesion: 1.0
Nodes (1): cosign verify-blob exits 0 → returns True.

### Community 590 - "Identity regexp must pin "
Cohesion: 1.0
Nodes (1): Identity regexp must pin to the release workflow, not the whole repo.

### Community 591 - "cosign verify-blob exits "
Cohesion: 1.0
Nodes (1): cosign verify-blob exits non-zero → returns False (abort install).

### Community 592 - "cosign not on PATH → retu"
Cohesion: 1.0
Nodes (1): cosign not on PATH → returns None (proceed with SHA-256 only).

### Community 593 - "cosign times out → return"
Cohesion: 1.0
Nodes (1): cosign times out → returns None (proceed with SHA-256 only).

### Community 594 - "cosign OSError → returns "
Cohesion: 1.0
Nodes (1): cosign OSError → returns None (proceed with SHA-256 only).

### Community 595 - "_install_tirith returns N"
Cohesion: 1.0
Nodes (1): _install_tirith returns None when cosign rejects the signature.

### Community 596 - "_install_tirith proceeds "
Cohesion: 1.0
Nodes (1): _install_tirith proceeds with SHA-256 only when cosign is not on PATH.

### Community 597 - "_install_tirith falls bac"
Cohesion: 1.0
Nodes (1): _install_tirith falls back to SHA-256 when cosign exists but fails to execute.

### Community 598 - "_install_tirith proceeds "
Cohesion: 1.0
Nodes (1): _install_tirith proceeds with SHA-256 when .sig/.pem downloads fail.

### Community 599 - "_install_tirith proceeds "
Cohesion: 1.0
Nodes (1): _install_tirith proceeds only when cosign explicitly passes (True).

### Community 600 - "Synchronous _resolve_tiri"
Cohesion: 1.0
Nodes (1): Synchronous _resolve_tirith_path persists failure to disk.

### Community 601 - "Successful install clears"
Cohesion: 1.0
Nodes (1): Successful install clears the disk failure marker.

### Community 602 - "When enabled_tools is Non"
Cohesion: 1.0
Nodes (1): When enabled_tools is None, all sandbox tools should be available.

### Community 603 - "When enabled_tools is [] "
Cohesion: 1.0
Nodes (1): When enabled_tools is [] (empty), all sandbox tools should be available.

### Community 604 - "When enabled_tools has no"
Cohesion: 1.0
Nodes (1): When enabled_tools has no overlap with SANDBOX_ALLOWED_TOOLS,         should fal

### Community 605 - "rg should skip .hub/ by d"
Cohesion: 1.0
Nodes (1): rg should skip .hub/ by default (no --hidden flag).

### Community 606 - "rg should find content in"
Cohesion: 1.0
Nodes (1): rg should find content in visible directories.

### Community 607 - "After max retries, the do"
Cohesion: 1.0
Nodes (1): After max retries, the download error should include exc_info.

### Community 608 - "When vision_analyze_tool "
Cohesion: 1.0
Nodes (1): When vision_analyze_tool encounters an error, it should log with exc_info.

### Community 609 - "Temp file cleanup failure"
Cohesion: 1.0
Nodes (1): Temp file cleanup failure should log warning with exc_info.

### Community 610 - "vision_analyze_tool shoul"
Cohesion: 1.0
Nodes (1): vision_analyze_tool should expand ~ in file paths.

### Community 611 - "A tilde path that doesn't"
Cohesion: 1.0
Nodes (1): A tilde path that doesn't resolve to a real file should fail gracefully.

### Community 612 - "Summarization should pick"
Cohesion: 1.0
Nodes (1): Summarization should pick up a backend that becomes available later in-process.

### Community 613 - "node-hide-console-windows"
Cohesion: 1.0
Nodes (1): node-hide-console-windows has a real MAL- advisory.

### Community 614 - "react should have zero MA"
Cohesion: 1.0
Nodes (1): react should have zero MAL- advisories.

### Community 615 - "Skills in deeply nested d"
Cohesion: 1.0
Nodes (1): Skills in deeply nested dirs (e.g. cli-tool/components/skills/dev/my-skill/)

### Community 616 - "skip_disabled=True ignore"
Cohesion: 1.0
Nodes (1): skip_disabled=True ignores the disabled set (for config UI).

### Community 617 - "Without skip_confirm, inp"
Cohesion: 1.0
Nodes (1): Without skip_confirm, input() is called for confirmation.

### Community 618 - "When launchd is running t"
Cohesion: 1.0
Nodes (1): When launchd is running the gateway, update should print         'auto-restart v

### Community 619 - "When no service manager i"
Cohesion: 1.0
Nodes (1): When no service manager is running but manual gateway is found, show manual rest

### Community 620 - "On Linux with systemd act"
Cohesion: 1.0
Nodes (1): On Linux with systemd active, update should restart via systemctl.

### Community 621 - "When no gateway is runnin"
Cohesion: 1.0
Nodes (1): When no gateway is running, update should skip the restart section entirely.

### Community 622 - "When user systemd is inac"
Cohesion: 1.0
Nodes (1): When user systemd is inactive but a system service exists, restart via system sc

### Community 623 - "When system service resta"
Cohesion: 1.0
Nodes (1): When system service restart fails, show the failure message.

### Community 624 - "When both user and system"
Cohesion: 1.0
Nodes (1): When both user and system services are active, both are restarted.

### Community 625 - "After launchd restart, th"
Cohesion: 1.0
Nodes (1): After launchd restart, the sweep must exclude the service PID.

### Community 626 - "After systemd restart, th"
Cohesion: 1.0
Nodes (1): After systemd restart, the sweep must exclude the service PID.

### Community 627 - "When both a service PID a"
Cohesion: 1.0
Nodes (1): When both a service PID and a manual PID exist, only the manual one         is k

### Community 628 - "Previously this code path"
Cohesion: 1.0
Nodes (1): Previously this code path raised NameError: 'is_coding_plan'.         Now it del

### Community 629 - "When fetch_api_models ret"
Cohesion: 1.0
Nodes (1): When fetch_api_models returns results, those are used instead of defaults.

### Community 630 - "Selecting 'Custom model' "
Cohesion: 1.0
Nodes (1): Selecting 'Custom model' lets user type a model name.

### Community 631 - "Second call within TTL re"
Cohesion: 1.0
Nodes (1): Second call within TTL returns cached result without API call.

### Community 632 - "After TTL expires, the AP"
Cohesion: 1.0
Nodes (1): After TTL expires, the API is called again.

### Community 633 - "Models already in vendor/"
Cohesion: 1.0
Nodes (1): Models already in vendor/model:tag format must not have their tag mangled.

### Community 634 - "Model in API but without "
Cohesion: 1.0
Nodes (1): Model in API but without context_length → defaults to 128000.

### Community 635 - "Persistent cache should b"
Cohesion: 1.0
Nodes (1): Persistent cache should be checked BEFORE API metadata.

### Community 636 - "Without base_url, cache l"
Cohesion: 1.0
Nodes (1): Without base_url, cache lookup is skipped.

### Community 637 - "Single-model servers: use"
Cohesion: 1.0
Nodes (1): Single-model servers: use the only model even if name doesn't match.

### Community 638 - "Fuzzy match: configured m"
Cohesion: 1.0
Nodes (1): Fuzzy match: configured model name is substring of endpoint model.

### Community 639 - "Explicit config_context_l"
Cohesion: 1.0
Nodes (1): Explicit config_context_length takes priority over everything.

### Community 640 - "config_context_length=0 s"
Cohesion: 1.0
Nodes (1): config_context_length=0 should be treated as unset.

### Community 641 - "config_context_length=Non"
Cohesion: 1.0
Nodes (1): config_context_length=None should be treated as unset.

### Community 642 - "Ensure 'qwen3.5:27b' is N"
Cohesion: 1.0
Nodes (1): Ensure 'qwen3.5:27b' is NOT reduced to '27b' during context length lookup.

### Community 643 - "On API failure with exist"
Cohesion: 1.0
Nodes (1): On API failure with existing cache, stale data is returned.

### Community 644 - "Models with canonical_slu"
Cohesion: 1.0
Nodes (1): Models with canonical_slug get indexed under both IDs.

### Community 645 - "Cache expires after _MODE"
Cohesion: 1.0
Nodes (1): Cache expires after _MODEL_CACHE_TTL seconds.

### Community 646 - "API returns JSON without "
Cohesion: 1.0
Nodes (1): API returns JSON without 'data' key — empty cache, no crash.

### Community 647 - "Same model, different con"
Cohesion: 1.0
Nodes (1): Same model, different context per provider.

### Community 648 - "Isolated config environme"
Cohesion: 1.0
Nodes (1): Isolated config environment with a writable config.yaml.

### Community 649 - "Base URL of the running s"
Cohesion: 1.0
Nodes (1): Base URL of the running server, e.g. ``http://127.0.0.1:12345``.

### Community 650 - "Symlinks pointing outside"
Cohesion: 1.0
Nodes (1): Symlinks pointing outside scripts/ must be rejected.

### Community 651 - "Estimated seconds remaini"
Cohesion: 1.0
Nodes (1): Estimated seconds remaining until reset, adjusted for elapsed time.

### Community 652 - "Error is expected to reso"
Cohesion: 1.0
Nodes (1): Error is expected to resolve on retry (with or without backoff).

### Community 653 - "Check if output is a real"
Cohesion: 1.0
Nodes (1): Check if output is a real terminal, safe against closed streams.

### Community 654 - "Normalize summary text to"
Cohesion: 1.0
Nodes (1): Normalize summary text to the current compaction handoff format.

### Community 655 - "Extract the call ID from "
Cohesion: 1.0
Nodes (1): Extract the call ID from a tool_call entry (dict or SimpleNamespace).

### Community 656 - "Short identifier for this"
Cohesion: 1.0
Nodes (1): Short identifier for this provider (e.g. 'builtin', 'honcho', 'hindsight').

### Community 657 - "Return True if this provi"
Cohesion: 1.0
Nodes (1): Return True if this provider is configured, has credentials, and is ready.

### Community 658 - "Initialize for a session."
Cohesion: 1.0
Nodes (1): Initialize for a session.          Called once at agent startup. May create reso

### Community 659 - "Return tool schemas this "
Cohesion: 1.0
Nodes (1): Return tool schemas this provider exposes.          Each schema follows the Open

### Community 660 - "Return metadata about all"
Cohesion: 1.0
Nodes (1): Return metadata about all loaded hooks.

### Community 661 - "True if at least one mess"
Cohesion: 1.0
Nodes (1): True if at least one message was sent/edited — signals the base         adapter

### Community 662 - "Strip MEDIA: directives a"
Cohesion: 1.0
Nodes (1): Strip MEDIA: directives and internal markers from text before display.

### Community 663 - "Split text into reasonabl"
Cohesion: 1.0
Nodes (1): Split text into reasonably sized chunks for fallback sends.

### Community 664 - "parallel-web"
Cohesion: 1.0
Nodes (1): parallel-web

### Community 665 - "Dynamic Reasoning Level"
Cohesion: 1.0
Nodes (1): Dynamic Reasoning Level

### Community 666 - "Session Naming Strategies"
Cohesion: 1.0
Nodes (1): Session Naming Strategies

### Community 667 - "HermesAgentBaseEnv"
Cohesion: 1.0
Nodes (1): HermesAgentBaseEnv

### Community 668 - "FastMCP - MCP Server Buil"
Cohesion: 1.0
Nodes (1): FastMCP - MCP Server Builder

### Community 669 - "Security Skills"
Cohesion: 1.0
Nodes (1): Security Skills

### Community 670 - "Popular Web Designs Skill"
Cohesion: 1.0
Nodes (1): Popular Web Designs Skill

### Community 671 - "Apple Design System"
Cohesion: 1.0
Nodes (1): Apple Design System

### Community 672 - "Typeform Design System"
Cohesion: 1.0
Nodes (1): Typeform Design System

### Community 673 - "Favicon 16x16"
Cohesion: 1.0
Nodes (1): Favicon 16x16

### Community 674 - "Apple Touch Icon"
Cohesion: 1.0
Nodes (1): Apple Touch Icon

### Community 675 - "Nous Research Logo"
Cohesion: 1.0
Nodes (1): Nous Research Logo

### Community 676 - "Hermes Agent Logo"
Cohesion: 1.0
Nodes (1): Hermes Agent Logo

### Community 677 - "Favicon SVG"
Cohesion: 1.0
Nodes (1): Favicon SVG

### Community 678 - "Favicon 32x32 PNG"
Cohesion: 1.0
Nodes (1): Favicon 32x32 PNG

### Community 679 - "Landing Page Favicon 16x1"
Cohesion: 1.0
Nodes (1): Landing Page Favicon 16x16

### Community 680 - "Landing Page Apple Touch "
Cohesion: 1.0
Nodes (1): Landing Page Apple Touch Icon

### Community 681 - "Landing Page Icon 192x192"
Cohesion: 1.0
Nodes (1): Landing Page Icon 192x192

### Community 682 - "Hermes Agent Banner"
Cohesion: 1.0
Nodes (1): Hermes Agent Banner

### Community 683 - "Landing Page Nous Logo"
Cohesion: 1.0
Nodes (1): Landing Page Nous Logo

### Community 684 - "Landing Page Icon 512x512"
Cohesion: 1.0
Nodes (1): Landing Page Icon 512x512

### Community 685 - "Landing Page Favicon 32x3"
Cohesion: 1.0
Nodes (1): Landing Page Favicon 32x32

### Community 686 - "Assets Banner"
Cohesion: 1.0
Nodes (1): Assets Banner

## Knowledge Gaps
- **4169 isolated node(s):** `Shared constants for Hermes Agent.  Import-safe module with no dependencies — ca`, `Return the Hermes home directory (default: ~/.hermes).      Reads HERMES_HOME en`, `Return the optional-skills directory, honoring package-manager wrappers.      Pa`, `Resolve a Hermes subdirectory with backward compatibility.      New installs get`, `Return a user-friendly display string for the current HERMES_HOME.      Uses ``~` (+4164 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **Thin community `default_soul.py / Default SOUL.md template `** (2 nodes): `default_soul.py`, `Default SOUL.md template seeded into HERMES_HOME on first run.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `index.tsx / handler()`** (2 nodes): `index.tsx`, `handler()`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `test_gateway_runtime_heal / test_runtime_health_lines`** (2 nodes): `test_gateway_runtime_health.py`, `test_runtime_health_lines_include_fatal_platform_and_startup_reason()`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `test_discord_media_metada / test_discord_media_method`** (2 nodes): `test_discord_media_metadata.py`, `test_discord_media_methods_accept_metadata_kwarg()`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `search_arxiv.py / search()`** (2 nodes): `search_arxiv.py`, `search()`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `MSE + L1 Sparsity Loss / SAE Training Workflow`** (2 nodes): `MSE + L1 Sparsity Loss`, `SAE Training Workflow`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Figma Design System / Miro Design System`** (2 nodes): `Figma Design System`, `Miro Design System`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Codebase Inspection Skill / Pygount Lines of Code Ana`** (2 nodes): `Codebase Inspection Skill`, `Pygount Lines of Code Analyzer`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Fallback Providers / Honcho Cross-Session Memo`** (2 nodes): `Fallback Providers`, `Honcho Cross-Session Memory`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Hermes Search / Session Recap`** (2 nodes): `Hermes Search`, `Session Recap`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Signal Messaging Platform / WhatsApp Messaging Platfo`** (2 nodes): `Signal Messaging Platform`, `WhatsApp Messaging Platform`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Home Assistant Messaging  / Open WebUI Messaging Plat`** (2 nodes): `Home Assistant Messaging Platform`, `Open WebUI Messaging Platform`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Load configuration from Y`** (1 nodes): `Load configuration from YAML file.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Normalize summary-model o`** (1 nodes): `Normalize summary-model output to a safe string.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Normalize summary text to`** (1 nodes): `Normalize summary text to include the expected prefix exactly once.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Validate and sanitize a s`** (1 nodes): `Validate and sanitize a session title.          - Strips leading/trailing whites`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Sanitize user input for s`** (1 nodes): `Sanitize user input for safe use in FTS5 MATCH queries.          FTS5 has its ow`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Current audio input RMS l`** (1 nodes): `Current audio input RMS level (0-32767). Updated each audio chunk.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Write numpy int16 audio d`** (1 nodes): `Write numpy int16 audio data to a WAV file.          Returns the file path.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Strip shell startup warni`** (1 nodes): `Strip shell startup warnings from the beginning of output.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Best-effort liveness chec`** (1 nodes): `Best-effort liveness check for host-visible PIDs.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Terminate a host-visible `** (1 nodes): `Terminate a host-visible PID without requiring the original process handle.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Return the writable sandb`** (1 nodes): `Return the writable sandbox temp dir for env-backed background tasks.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Acquire an exclusive file`** (1 nodes): `Acquire an exclusive file lock for read-modify-write safety.          Uses a sep`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Read a memory file and sp`** (1 nodes): `Read a memory file and split into entries.          No file locking needed: _wri`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Write entries to a memory`** (1 nodes): `Write entries to a memory file using atomic temp-file + rename.          Previou`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Extract text from a ToolR`** (1 nodes): `Extract text from a ToolResultContent block.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Return ErrorData (MCP spe`** (1 nodes): `Return ErrorData (MCP spec) or raise as fallback.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Validate and normalize a `** (1 nodes): `Validate and normalize a todo item.          Ensures required fields exist and s`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Read a file with paginati`** (1 nodes): `Read a file with pagination support.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Write content to a file, `** (1 nodes): `Write content to a file, creating directories as needed.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Replace text in a file us`** (1 nodes): `Replace text in a file using fuzzy matching.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Apply a V4A format patch.`** (1 nodes): `Apply a V4A format patch.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Search for content or fil`** (1 nodes): `Search for content or files.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Parse git --shortstat out`** (1 nodes): `Parse git --shortstat output into entry dict.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Short, human-readable nam`** (1 nodes): `Short, human-readable name shown in logs and diagnostics.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Return True when all requ`** (1 nodes): `Return True when all required env vars / credentials are present.          Calle`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Create a cloud browser se`** (1 nodes): `Create a cloud browser session and return session metadata.          Must return`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Release / terminate a clo`** (1 nodes): `Release / terminate a cloud session by its provider session ID.          Returns`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Best-effort session teard`** (1 nodes): `Best-effort session teardown during process exit.          Called from atexit /`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Release backend resources`** (1 nodes): `Release backend resources (container, instance, connection).`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Append stdin_data as a sh`** (1 nodes): `Append stdin_data as a shell heredoc to the command string.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Return replacement text f`** (1 nodes): `Return replacement text for a completion.          When the user has already typ`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Extract the current word `** (1 nodes): `Extract the current word if it looks like a file path.          Returns the path`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Yield Completion objects `** (1 nodes): `Yield Completion objects for file paths matching *word*.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Extract a bare ``@`` toke`** (1 nodes): `Extract a bare ``@`` token for context reference completions.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Yield Claude Code-style @`** (1 nodes): `Yield Claude Code-style @ context completions.          Bare ``@`` or ``@partial`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Create config from enviro`** (1 nodes): `Create config from environment variables (fallback).`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Create config from the re`** (1 nodes): `Create config from the resolved Honcho config path.          Resolution: $HERMES`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Return the git repo root `** (1 nodes): `Return the git repo root directory name, or None if not in a repo.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Get the Honcho client, in`** (1 nodes): `Get the Honcho client, initializing if needed.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Format local messages as `** (1 nodes): `Format local messages as an XML transcript for Honcho file upload.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Normalize Honcho card pay`** (1 nodes): `Normalize Honcho card payloads into a plain list of strings.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `docusaurus.config.ts`** (1 nodes): `docusaurus.config.ts`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `sidebars.ts`** (1 nodes): `sidebars.ts`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `_run_async should still w`** (1 nodes): `_run_async should still work when called from inside an         already-running`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `test_minisweagent_path.py`** (1 nodes): `test_minisweagent_path.py`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Lazy-import execute_code `** (1 nodes): `Lazy-import execute_code to avoid pulling in firecrawl at collection time.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Read then write with no e`** (1 nodes): `Read then write with no external modification — no warning.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Read, then external modif`** (1 nodes): `Read, then external modify, then write — should warn.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Writing a file that was n`** (1 nodes): `Writing a file that was never read — no warning.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Creating a new file — no `** (1 nodes): `Creating a new file — no warning.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Task A reads, file change`** (1 nodes): `Task A reads, file changes, Task B writes — no warning for B.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Patch should warn if the `** (1 nodes): `Patch should warn if the target file changed since last read.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Patch with no external ch`** (1 nodes): `Patch with no external changes — no warning.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `A read that returns >max `** (1 nodes): `A read that returns >max chars is rejected.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Normal-sized reads pass t`** (1 nodes): `Normal-sized reads pass through fine.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Content just under the li`** (1 nodes): `Content just under the limit should pass through fine.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Second read of same file+`** (1 nodes): `Second read of same file+range returns dedup stub.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `After the file is modifie`** (1 nodes): `After the file is modified, dedup returns full content.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Same file but different o`** (1 nodes): `Same file but different offset/limit should not dedup.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Different task_ids have s`** (1 nodes): `Different task_ids have separate dedup caches.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `After reset_file_dedup, t`** (1 nodes): `After reset_file_dedup, the same read returns full content.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `reset_file_dedup(None) cl`** (1 nodes): `reset_file_dedup(None) clears all tasks.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `reset_file_dedup does NOT`** (1 nodes): `reset_file_dedup does NOT affect the consecutive-read counter.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `A config value of 50 shou`** (1 nodes): `A config value of 50 should reject reads over 50 chars.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `A config value of 500K sh`** (1 nodes): `A config value of 500K should allow reads up to 500K chars.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `When tasks array is provi`** (1 nodes): `When tasks array is provided, top-level goal/context/toolsets are ignored.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `When delegation.provider `** (1 nodes): `When delegation.provider is set, full credentials are resolved.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Nous provider resolves No`** (1 nodes): `Nous provider resolves Nous Portal base_url and api_key.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `When provider resolution `** (1 nodes): `When provider resolution fails, ValueError is raised with helpful message.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `When provider resolves bu`** (1 nodes): `When provider resolves but has no API key, ValueError is raised.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `When delegation.provider `** (1 nodes): `When delegation.provider is configured, child agent gets resolved credentials.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Parent on Nous, subagent `** (1 nodes): `Parent on Nous, subagent on OpenRouter — full credential switch.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `When delegation config is`** (1 nodes): `When delegation config is empty, child inherits parent credentials.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `When credential resolutio`** (1 nodes): `When credential resolution fails, delegate_task returns a JSON error.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `In batch mode, all childr`** (1 nodes): `In batch mode, all children receive the resolved credentials.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Setting only model (no pr`** (1 nodes): `Setting only model (no provider) changes model but keeps parent credentials.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Shared patches for pre-na`** (1 nodes): `Shared patches for pre-navigation tests that pass the SSRF check.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Shared patches for redire`** (1 nodes): `Shared patches for redirect tests.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `On Windows, the old check`** (1 nodes): `On Windows, the old check incorrectly blocks valid subpaths.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `tirith block goes through`** (1 nodes): `tirith block goes through approval flow (user gets prompted).`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `tirith block + dangerous `** (1 nodes): `tirith block + dangerous pattern → combined approval prompt.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `In gateway mode, tirith b`** (1 nodes): `In gateway mode, tirith block should return approval_required.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Both tirith warn and dang`** (1 nodes): `Both tirith warn and dangerous → single approval_required with both keys.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Non-ImportError exception`** (1 nodes): `Non-ImportError exceptions from tirith wrapper should propagate.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `After a failed download, `** (1 nodes): `After a failed download, subsequent resolves must not retry.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `After cached miss, check_`** (1 nodes): `After cached miss, check_command_security hits OSError → fail_open.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `An explicit tirith_path t`** (1 nodes): `An explicit tirith_path that doesn't exist must NOT trigger download.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `An explicit ~/path that d`** (1 nodes): `An explicit ~/path that doesn't exist must NOT trigger download.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `The default bare 'tirith'`** (1 nodes): `The default bare 'tirith' SHOULD trigger auto-download.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `cosign verify-blob exits `** (1 nodes): `cosign verify-blob exits 0 → returns True.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Identity regexp must pin `** (1 nodes): `Identity regexp must pin to the release workflow, not the whole repo.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `cosign verify-blob exits `** (1 nodes): `cosign verify-blob exits non-zero → returns False (abort install).`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `cosign not on PATH → retu`** (1 nodes): `cosign not on PATH → returns None (proceed with SHA-256 only).`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `cosign times out → return`** (1 nodes): `cosign times out → returns None (proceed with SHA-256 only).`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `cosign OSError → returns `** (1 nodes): `cosign OSError → returns None (proceed with SHA-256 only).`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `_install_tirith returns N`** (1 nodes): `_install_tirith returns None when cosign rejects the signature.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `_install_tirith proceeds `** (1 nodes): `_install_tirith proceeds with SHA-256 only when cosign is not on PATH.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `_install_tirith falls bac`** (1 nodes): `_install_tirith falls back to SHA-256 when cosign exists but fails to execute.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `_install_tirith proceeds `** (1 nodes): `_install_tirith proceeds with SHA-256 when .sig/.pem downloads fail.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `_install_tirith proceeds `** (1 nodes): `_install_tirith proceeds only when cosign explicitly passes (True).`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Synchronous _resolve_tiri`** (1 nodes): `Synchronous _resolve_tirith_path persists failure to disk.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Successful install clears`** (1 nodes): `Successful install clears the disk failure marker.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `When enabled_tools is Non`** (1 nodes): `When enabled_tools is None, all sandbox tools should be available.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `When enabled_tools is [] `** (1 nodes): `When enabled_tools is [] (empty), all sandbox tools should be available.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `When enabled_tools has no`** (1 nodes): `When enabled_tools has no overlap with SANDBOX_ALLOWED_TOOLS,         should fal`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `rg should skip .hub/ by d`** (1 nodes): `rg should skip .hub/ by default (no --hidden flag).`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `rg should find content in`** (1 nodes): `rg should find content in visible directories.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `After max retries, the do`** (1 nodes): `After max retries, the download error should include exc_info.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `When vision_analyze_tool `** (1 nodes): `When vision_analyze_tool encounters an error, it should log with exc_info.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Temp file cleanup failure`** (1 nodes): `Temp file cleanup failure should log warning with exc_info.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `vision_analyze_tool shoul`** (1 nodes): `vision_analyze_tool should expand ~ in file paths.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `A tilde path that doesn't`** (1 nodes): `A tilde path that doesn't resolve to a real file should fail gracefully.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Summarization should pick`** (1 nodes): `Summarization should pick up a backend that becomes available later in-process.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `node-hide-console-windows`** (1 nodes): `node-hide-console-windows has a real MAL- advisory.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `react should have zero MA`** (1 nodes): `react should have zero MAL- advisories.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Skills in deeply nested d`** (1 nodes): `Skills in deeply nested dirs (e.g. cli-tool/components/skills/dev/my-skill/)`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `skip_disabled=True ignore`** (1 nodes): `skip_disabled=True ignores the disabled set (for config UI).`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Without skip_confirm, inp`** (1 nodes): `Without skip_confirm, input() is called for confirmation.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `When launchd is running t`** (1 nodes): `When launchd is running the gateway, update should print         'auto-restart v`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `When no service manager i`** (1 nodes): `When no service manager is running but manual gateway is found, show manual rest`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `On Linux with systemd act`** (1 nodes): `On Linux with systemd active, update should restart via systemctl.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `When no gateway is runnin`** (1 nodes): `When no gateway is running, update should skip the restart section entirely.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `When user systemd is inac`** (1 nodes): `When user systemd is inactive but a system service exists, restart via system sc`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `When system service resta`** (1 nodes): `When system service restart fails, show the failure message.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `When both user and system`** (1 nodes): `When both user and system services are active, both are restarted.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `After launchd restart, th`** (1 nodes): `After launchd restart, the sweep must exclude the service PID.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `After systemd restart, th`** (1 nodes): `After systemd restart, the sweep must exclude the service PID.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `When both a service PID a`** (1 nodes): `When both a service PID and a manual PID exist, only the manual one         is k`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Previously this code path`** (1 nodes): `Previously this code path raised NameError: 'is_coding_plan'.         Now it del`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `When fetch_api_models ret`** (1 nodes): `When fetch_api_models returns results, those are used instead of defaults.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Selecting 'Custom model' `** (1 nodes): `Selecting 'Custom model' lets user type a model name.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Second call within TTL re`** (1 nodes): `Second call within TTL returns cached result without API call.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `After TTL expires, the AP`** (1 nodes): `After TTL expires, the API is called again.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Models already in vendor/`** (1 nodes): `Models already in vendor/model:tag format must not have their tag mangled.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Model in API but without `** (1 nodes): `Model in API but without context_length → defaults to 128000.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Persistent cache should b`** (1 nodes): `Persistent cache should be checked BEFORE API metadata.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Without base_url, cache l`** (1 nodes): `Without base_url, cache lookup is skipped.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Single-model servers: use`** (1 nodes): `Single-model servers: use the only model even if name doesn't match.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Fuzzy match: configured m`** (1 nodes): `Fuzzy match: configured model name is substring of endpoint model.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Explicit config_context_l`** (1 nodes): `Explicit config_context_length takes priority over everything.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `config_context_length=0 s`** (1 nodes): `config_context_length=0 should be treated as unset.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `config_context_length=Non`** (1 nodes): `config_context_length=None should be treated as unset.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Ensure 'qwen3.5:27b' is N`** (1 nodes): `Ensure 'qwen3.5:27b' is NOT reduced to '27b' during context length lookup.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `On API failure with exist`** (1 nodes): `On API failure with existing cache, stale data is returned.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Models with canonical_slu`** (1 nodes): `Models with canonical_slug get indexed under both IDs.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Cache expires after _MODE`** (1 nodes): `Cache expires after _MODEL_CACHE_TTL seconds.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `API returns JSON without `** (1 nodes): `API returns JSON without 'data' key — empty cache, no crash.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Same model, different con`** (1 nodes): `Same model, different context per provider.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Isolated config environme`** (1 nodes): `Isolated config environment with a writable config.yaml.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Base URL of the running s`** (1 nodes): `Base URL of the running server, e.g. ``http://127.0.0.1:12345``.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Symlinks pointing outside`** (1 nodes): `Symlinks pointing outside scripts/ must be rejected.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Estimated seconds remaini`** (1 nodes): `Estimated seconds remaining until reset, adjusted for elapsed time.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Error is expected to reso`** (1 nodes): `Error is expected to resolve on retry (with or without backoff).`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Check if output is a real`** (1 nodes): `Check if output is a real terminal, safe against closed streams.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Normalize summary text to`** (1 nodes): `Normalize summary text to the current compaction handoff format.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Extract the call ID from `** (1 nodes): `Extract the call ID from a tool_call entry (dict or SimpleNamespace).`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Short identifier for this`** (1 nodes): `Short identifier for this provider (e.g. 'builtin', 'honcho', 'hindsight').`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Return True if this provi`** (1 nodes): `Return True if this provider is configured, has credentials, and is ready.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Initialize for a session.`** (1 nodes): `Initialize for a session.          Called once at agent startup. May create reso`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Return tool schemas this `** (1 nodes): `Return tool schemas this provider exposes.          Each schema follows the Open`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Return metadata about all`** (1 nodes): `Return metadata about all loaded hooks.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `True if at least one mess`** (1 nodes): `True if at least one message was sent/edited — signals the base         adapter`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Strip MEDIA: directives a`** (1 nodes): `Strip MEDIA: directives and internal markers from text before display.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Split text into reasonabl`** (1 nodes): `Split text into reasonably sized chunks for fallback sends.`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `parallel-web`** (1 nodes): `parallel-web`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Dynamic Reasoning Level`** (1 nodes): `Dynamic Reasoning Level`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Session Naming Strategies`** (1 nodes): `Session Naming Strategies`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `HermesAgentBaseEnv`** (1 nodes): `HermesAgentBaseEnv`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `FastMCP - MCP Server Buil`** (1 nodes): `FastMCP - MCP Server Builder`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Security Skills`** (1 nodes): `Security Skills`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Popular Web Designs Skill`** (1 nodes): `Popular Web Designs Skill`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Apple Design System`** (1 nodes): `Apple Design System`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Typeform Design System`** (1 nodes): `Typeform Design System`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Favicon 16x16`** (1 nodes): `Favicon 16x16`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Apple Touch Icon`** (1 nodes): `Apple Touch Icon`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Nous Research Logo`** (1 nodes): `Nous Research Logo`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Hermes Agent Logo`** (1 nodes): `Hermes Agent Logo`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Favicon SVG`** (1 nodes): `Favicon SVG`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Favicon 32x32 PNG`** (1 nodes): `Favicon 32x32 PNG`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Landing Page Favicon 16x1`** (1 nodes): `Landing Page Favicon 16x16`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Landing Page Apple Touch `** (1 nodes): `Landing Page Apple Touch Icon`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Landing Page Icon 192x192`** (1 nodes): `Landing Page Icon 192x192`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Hermes Agent Banner`** (1 nodes): `Hermes Agent Banner`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Landing Page Nous Logo`** (1 nodes): `Landing Page Nous Logo`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Landing Page Icon 512x512`** (1 nodes): `Landing Page Icon 512x512`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Landing Page Favicon 32x3`** (1 nodes): `Landing Page Favicon 32x32`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Assets Banner`** (1 nodes): `Assets Banner`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What are the core architectural components of hermes-agent?**
  _Top-level structure of the project._
- **How do skills interact with the tool system?**
  _Skills and tools are the two main extension points._
- **What is the relationship between gateway and CLI modules?**
  _Both orchestrate the agent but for different platforms._