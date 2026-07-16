Проведен анализ файлов проекта для выявления неиспользуемых изображений в директории [`mkdocs/img`](mkdocs/img).

### Методология:
1.  **Поиск ссылок:** Все файлы `*.md` в папке `mkdocs` были просканированы на наличие синтаксиса изображений Markdown `![]()` и HTML тегов `<img>`.
2.  **Инвентаризация файлов:** Составлен полный список файлов в директории [`mkdocs/img`](mkdocs/img), включая поддиректории.
3.  **Сопоставление:** Пути из файлов были нормализованы и сопоставлены с реальными файлами на диске.

### Список неиспользуемых файлов в `mkdocs/img`:
Ниже перечислены файлы, на которые нет ссылок ни в одном `.md` файле проекта:

**Корневая папка `mkdocs/img/`:**
*   (Все файлы используются)

**Папка `mkdocs/img/bake-tutor-1/`:**
*   [`bake-tutor-1/add-normal-map-node.png`](mkdocs/img/bake-tutor-1/add-normal-map-node.png)
*   [`bake-tutor-1/cycles-to-eevee.png`](mkdocs/img/bake-tutor-1/cycles-to-eevee.png)
*   [`bake-tutor-1/remove-preview-node.png`](mkdocs/img/bake-tutor-1/remove-preview-node.png)
*   [`bake-tutor-1/surface-settings.png`](mkdocs/img/bake-tutor-1/surface-settings.png)

**Папка `mkdocs/img/bbq-screens/npanel/`:**
*   [`bbq-screens/npanel/bevel_to_vc_op_prop.png`](mkdocs/img/bbq-screens/npanel/bevel_to_vc_op_prop.png)
*   [`bbq-screens/npanel/examples.png`](mkdocs/img/bbq-screens/npanel/examples.png)
*   [`bbq-screens/npanel/help.png`](mkdocs/img/bbq-screens/npanel/help.png)
*   [`bbq-screens/npanel/main_panel.png`](mkdocs/img/bbq-screens/npanel/main_panel.png) *(Примечание: используется версия из подпапки mainpanel, эта копия в npanel не используется)*
*   [`bbq-screens/npanel/main-redner-preview.png`](mkdocs/img/bbq-screens/npanel/main-redner-preview.png)
*   [`bbq-screens/npanel/preferences-assign-bevel-boundary.gif`](mkdocs/img/bbq-screens/npanel/preferences-assign-bevel-boundary.gif)
*   [`bbq-screens/npanel/preferences-confirm-cycles.png`](mkdocs/img/bbq-screens/npanel/preferences-confirm-cycles.png)
*   [`bbq-screens/npanel/preferences.png`](mkdocs/img/bbq-screens/npanel/preferences.png)
*   [`bbq-screens/npanel/shader_preview_example.png`](mkdocs/img/bbq-screens/npanel/shader_preview_example.png)
*   [`bbq-screens/npanel/show_max_bevel_by_mat_popup.png`](mkdocs/img/bbq-screens/npanel/show_max_bevel_by_mat_popup.png)
*   [`bbq-screens/npanel/show_max_bevel_invoke.png`](mkdocs/img/bbq-screens/npanel/show_max_bevel_invoke.png)
*   [`bbq-screens/npanel/tools_panel.png`](mkdocs/img/bbq-screens/npanel/tools_panel.png)
*   [`bbq-screens/npanel/ZenBBQ_LiveBooleanGIF.gif`](mkdocs/img/bbq-screens/npanel/ZenBBQ_LiveBooleanGIF.gif)

**Папка `mkdocs/img/icons/`:**
*   [`icons/a.png`](mkdocs/img/icons/a.png)
*   [`icons/display.png`](mkdocs/img/icons/display.png)
*   [`icons/download.png`](mkdocs/img/icons/download.png)
*   [`icons/m.png`](mkdocs/img/icons/m.png)
*   [`icons/minus.png`](mkdocs/img/icons/minus.png)
*   [`icons/plus.png`](mkdocs/img/icons/plus.png)
*   [`icons/select.png`](mkdocs/img/icons/select.png)
*   [`icons/trash.png`](mkdocs/img/icons/trash.png)
*   [`icons/services/Superhive-32.png`](mkdocs/img/icons/services/Superhive-32.png)
*   [`icons/services/discord-32.png`](mkdocs/img/icons/services/discord-32.png)
*   [`icons/services/gumroad-32.png`](mkdocs/img/icons/services/gumroad-32.png)

**Папка `mkdocs/img/promo-images/`:**
*   [`promo-images/Carburetor_Before_After.jpg`](mkdocs/img/promo-images/Carburetor_Before_After.jpg)
*   [`promo-images/Carburetor_Colorized_Display.jpg`](mkdocs/img/promo-images/Carburetor_Colorized_Display.jpg)
*   [`promo-images/Carburetor_Controllable_Radii.jpg`](mkdocs/img/promo-images/Carburetor_Controllable_Radii.jpg)