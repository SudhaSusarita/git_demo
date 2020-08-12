git:dev -> git dev
git: featured_dev -> local dev

When you have accidentally committed changes in dev branch instead of local dev. 

Fix:

create a new branch from dev branch wch has ur code
now the local branch also has your modified code

use >git logs --oneline
displays all the commit msgs and id
choose the version to have to make as head(normally head points to current latest correct commit)
if its not the crcct head then reset it by
>git reset --hard<correct commit id>

now go to git : dev  branch
repeat line 11-15
now >git push --force (* alwys make sure if its in right commit id before forcing it to push)

Also go to dev local and push those changes to its own branch