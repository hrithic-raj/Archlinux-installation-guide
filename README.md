◄ 0s ◎ ls ~/.config/caelestia/                                                ⌂ 14:27
󱁻 hypr-user.conf
󱁻 hypr-vars.conf
                                                                                     
◄ 0s ◎ ls -la ~/.config/caelestia/hypr-user.conf                              ⌂ 14:31
.rw-r--r-- 0 hrj 31 May 14:20 󱁻 /home/hrj/.config/caelestia/hypr-user.conf
                                                                                     
◄ 0s ◎ ls -la ~/.config/caelestia/hypr-vars.conf                              ⌂ 14:32
.rw-r--r-- 0 hrj 31 May 14:20 󱁻 /home/hrj/.config/caelestia/hypr-vars.conf
                                                                                     
◄ 0s ◎ which swww                                                             ⌂ 14:32
which: no swww in (/usr/local/bin:/usr/bin)
                                                                                     
◄ 0s ○ pgrep swww-daemon                                                      ⌂ 14:32
                                                                                     
◄ 0s ○ which hyprpaper                                                        ⌂ 14:33
which: no hyprpaper in (/usr/local/bin:/usr/bin)
                                                                                     
◄ 0s ○ grep -Ri "swww\|hyprpaper" ~/.local/share/caelestia/                   ⌂ 14:33
                                                                                     
◄ 0s ○ grep -Ri "swww\|hyprpaper" ~/.local/share/caelestia/                   ⌂ 14:35
                                                                                     
◄ 0s ○ hyprctl reload                                                         ⌂ 14:36
ok
                                                                                     
◄ 0s ◎ hyprctl log -f                                                         ⌂ 14:36
only 'rollinglog' command supports '--follow' option
                                                                                     
◄ 0s ○ journalctl --user -n 100 | grep -i hypr                                ⌂ 14:37
May 31 14:20:05 HRJ systemd[2039]: Starting Portal service (Hyprland implementation)...
May 31 14:20:05 HRJ systemd[2039]: Started Portal service (Hyprland implementation).
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG] Initializing xdph...
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG] XDG_CURRENT_DESKTOP set to Hyprland
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG] Gathering exported interfaces
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wl_seat (ver 9)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wl_data_device_manager (ver 3)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wl_compositor (ver 6)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wl_subcompositor (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wl_shm (ver 2)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wp_viewporter (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wp_tearing_control_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wp_fractional_scale_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zxdg_output_manager_v1 (ver 3)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wp_cursor_shape_manager_v1 (ver 2)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zwp_idle_inhibit_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zwp_relative_pointer_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zxdg_decoration_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wp_alpha_modifier_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zwlr_gamma_control_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: ext_foreign_toplevel_list_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zwp_pointer_gestures_v1 (ver 3)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zwlr_foreign_toplevel_manager_v1 (ver 3)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG] [toplevel] (activate) locks: 1
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zwp_keyboard_shortcuts_inhibit_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zwp_text_input_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zwp_text_input_manager_v3 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zwp_pointer_constraints_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zwlr_output_power_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: xdg_activation_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: ext_idle_notifier_v1 (ver 2)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: hyprland_lock_notifier_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: ext_session_lock_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zwp_input_method_manager_v2 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zwp_virtual_keyboard_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zwlr_virtual_pointer_manager_v1 (ver 2)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zwlr_output_manager_v1 (ver 4)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: org_kde_kwin_server_decoration_manager (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: hyprland_focus_grab_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zwp_tablet_manager_v2 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zwlr_layer_shell_v1 (ver 5)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wp_presentation (ver 2)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: xdg_wm_base (ver 7)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zwlr_data_control_manager_v1 (ver 2)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zwp_primary_selection_device_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: xwayland_shell_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: hyprland_toplevel_mapping_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG] [toplevel mapping] registered manager
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: hyprland_global_shortcuts_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG] [globalshortcuts] registered
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: xdg_wm_dialog_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wp_single_pixel_buffer_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wp_security_context_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: hyprland_ctm_control_manager_v1 (ver 2)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: hyprland_surface_manager_v1 (ver 2)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wp_content_type_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: xdg_toplevel_tag_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: xdg_system_bell_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: ext_workspace_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: ext_data_control_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wp_pointer_warp_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wp_fifo_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zxdg_exporter_v2 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zxdg_importer_v2 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wp_commit_timing_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: zwlr_screencopy_manager_v1 (ver 3)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG] [pipewire] connected
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG] [screencopy] init successful
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: hyprland_toplevel_export_manager_v1 (ver 2)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: ext_output_image_capture_source_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: ext_foreign_toplevel_image_capture_source_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: ext_image_copy_capture_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wp_color_manager_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wp_drm_lease_device_v1 (ver 1)
May 31 14:20:05 HRJ xdg-desktop-portal-hyprland[2361]: [LOG]  | Got interface: wp_linux_drm_syncobj_manager_v1 (ver 1)
