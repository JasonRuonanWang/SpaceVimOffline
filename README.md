diff --git a/autoload/SpaceVim.vim b/autoload/SpaceVim.vim
index 6bbeb026..af9a72db 100644
--- a/autoload/SpaceVim.vim
+++ b/autoload/SpaceVim.vim
@@ -940,7 +940,7 @@ let g:spacevim_plugin_manager_processes = 16
 " >
 "   let g:spacevim_checkinstall = 1
 " <
-let g:spacevim_checkinstall            = 1
+let g:spacevim_checkinstall            = 0
 ""
 " @section vimcompatible, options-vimcompatible
 " @parentsection options
diff --git a/docs/install.sh b/docs/install.sh
index 2aac8f91..5cfc0114 100755
--- a/docs/install.sh
+++ b/docs/install.sh
@@ -392,7 +392,7 @@ main () {
                 ;;
             --install|-i)
                 welcome
-                fetch_repo
+#                fetch_repo
                 if [ $# -eq 2 ]
                 then
                     case $2 in
@@ -421,7 +421,7 @@ main () {
                 ;;
             --no-fonts)
                 welcome
-                fetch_repo
+#                fetch_repo
                 install_vim
                 install_neovim
                 install_done
@@ -433,7 +433,7 @@ main () {
         esac
     else
         welcome
-        fetch_repo
+#        fetch_repo
         install_vim
         install_neovim
         install_fonts
