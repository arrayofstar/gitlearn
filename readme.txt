Git is a distributed version control system.
Git is free software distributed under the GPL.
Git has a mutable index called stage.
Git tracks changes of files.
Creating a new branch is quick & simaple..
do some change.
do some other change.

# Git���
## �����汾��

> mkdir learngit
> cd learngit
> pwd

��ʼ��һ��Git�ֿ⣬ʹ��git init���
����ļ���Git�ֿ⣬��������
1. ʹ������git add <file>��ע�⣬�ɷ������ʹ�ã���Ӷ���ļ���
2. ʹ������git commit -m <message>����ɡ�

# ʱ�������

- Ҫ��ʱ���չ�������״̬��ʹ��git status���
- ���git status���������ļ����޸Ĺ�����git diff���Բ鿴�޸����ݡ�

## �汾����

- HEADָ��İ汾���ǵ�ǰ�汾����ˣ�Git���������ڰ汾����ʷ֮�䴩��ʹ������git reset --hard commit_id��
- ����ǰ����git log���Բ鿴�ύ��ʷ���Ա�ȷ��Ҫ���˵��ĸ��汾��
- Ҫ�ط�δ������git reflog�鿴������ʷ���Ա�ȷ��Ҫ�ص�δ�����ĸ��汾��

## ���������ݴ���

- ��

## �����޸�

$ git add readme.txt
$ git status
$ git commit -m "git tracks changes"
$ git status

## �����޸�

- ����1����������˹�����ĳ���ļ������ݣ���ֱ�Ӷ������������޸�ʱ��������git checkout -- file��
- ����2�����㲻�������˹�����ĳ���ļ������ݣ�����ӵ����ݴ���ʱ���붪���޸ģ�����������һ��������git reset HEAD <file>���ͻص��˳���1���ڶ���������1������
- ����3���Ѿ��ύ�˲����ʵ��޸ĵ��汾��ʱ����Ҫ���������ύ���ο��汾����һ�ڣ�����ǰ����û�����͵�Զ�̿⡣

## ɾ���ļ�

- ����git rm����ɾ��һ���ļ������һ���ļ��Ѿ����ύ���汾�⣬��ô����Զ���õ�����ɾ������ҪС�ģ���ֻ�ָܻ��ļ������°汾����ᶪʧ���һ���ύ�����޸ĵ����ݡ�

# Զ�ֿ̲�

- $ ssh-keygen -t rsa -C "youremail@example.com"
- ���û���Ŀ¼���ҵ�.sshĿ¼��������id_rsa��id_rsa.pub�����ļ�������������SSH Key����Կ�ԣ�id_rsa��˽Կ������й¶��ȥ��id_rsa.pub�ǹ�Կ�����Է��ĵظ����κ��ˡ�

## ���Զ�̿�

- Ҫ����һ��Զ�̿⣬ʹ������git remote add origin git@server-name:path/repo-name.git��

- ����һ��Զ�̿�ʱ�����Զ�̿�ָ��һ�����֣�origin��Ĭ��ϰ��������

- ������ʹ������git push -u origin master��һ������master��֧���������ݣ�

- �˺�ÿ�α����ύ��ֻҪ�б�Ҫ���Ϳ���ʹ������git push origin master���������޸ģ�

- �ֲ�ʽ�汾ϵͳ�����ô�֮һ���ڱ��ع�����ȫ����Ҫ����Զ�̿�Ĵ��ڣ�Ҳ������û������������������������SVN��û��������ʱ���Ǿܾ��ɻ�ģ����������ʱ���ٰѱ����ύ����һ�¾������ͬ��������̫�����ˣ�

## ��Զ�̿��¡

- Ҫ��¡һ���ֿ⣬���ȱ���֪���ֿ�ĵ�ַ��Ȼ��ʹ��git clone�����¡��

- Git֧�ֶ���Э�飬����https����sshЭ���ٶ���졣

# ��֧����

## ������ϲ���֧

Git��������ʹ�÷�֧��

- �鿴��֧��git branch

- ������֧��git branch <name>

- �л���֧��git checkout <name>����git switch <name>

- ����+�л���֧��git checkout -b <name>����git switch -c <name>

- �ϲ�ĳ��֧����ǰ��֧��git merge <name>

- ɾ����֧��git branch -d <name>

## �����ͻ

- ��Git�޷��Զ��ϲ���֧ʱ���ͱ������Ƚ����ͻ�������ͻ�����ύ���ϲ���ɡ�

- �����ͻ���ǰ�Git�ϲ�ʧ�ܵ��ļ��ֶ��༭Ϊ����ϣ�������ݣ����ύ��

- ��git log --graph������Կ�����֧�ϲ�ͼ��

- ��--pretty=oneline --abbrev-commit������Կ��ĸ���ȫ��

## ��֧�������

- Git��֧ʮ��ǿ�����Ŷӿ�����Ӧ�ó��Ӧ�á�

- �ϲ���֧ʱ������--no-ff�����Ϳ�������ͨģʽ�ϲ����ϲ������ʷ�з�֧���ܿ��������������ϲ�����fast forward�ϲ��Ϳ����������������ϲ���


## Bug��֧

�޸�bugʱ�����ǻ�ͨ�������µ�bug��֧�����޸���Ȼ��ϲ������ɾ����

����ͷ����û�����ʱ���Ȱѹ����ֳ�git stashһ�£�Ȼ��ȥ�޸�bug���޸�����git stash pop���ص������ֳ���

��master��֧���޸���bug����Ҫ�ϲ�����ǰdev��֧��������git cherry-pick <commit>�����bug�ύ���޸ġ����ơ�����ǰ��֧�������ظ��Ͷ���

## Feature��֧

- ����һ����feature������½�һ����֧��
- $ git switch -c feature-vulcan

- ���Ҫ����һ��û�б��ϲ����ķ�֧������ͨ��git branch -D <name>ǿ��ɾ����

## ����Э��

- �鿴Զ�̿����Ϣ����git remote -v��

1.master��֧������֧�����Ҫʱ����Զ��ͬ����
2.dev��֧�ǿ�����֧���Ŷ����г�Ա����Ҫ�����湤��������Ҳ��Ҫ��Զ��ͬ����
3.bug��ֻ֧�����ڱ����޸�bug����û��Ҫ�Ƶ�Զ���ˣ������ϰ�Ҫ������ÿ�ܵ����޸��˼���bug��
4.feature��֧�Ƿ��Ƶ�Զ�̣�ȡ�������Ƿ�����С�����������濪����

- �����½��ķ�֧��������͵�Զ�̣��������˾��ǲ��ɼ��ģ�

- �ӱ������ͷ�֧��ʹ��git push origin branch-name���������ʧ�ܣ�����git pullץȡԶ�̵����ύ��

- �ڱ��ش�����Զ�̷�֧��Ӧ�ķ�֧��ʹ��git checkout -b branch-name origin/branch-name�����غ�Զ�̷�֧���������һ�£�

- �������ط�֧��Զ�̷�֧�Ĺ�����ʹ��git branch --set-upstream branch-name origin/branch-name��

- ��Զ��ץȡ��֧��ʹ��git pull������г�ͻ��Ҫ�ȴ����ͻ��

## Rebase

- rebase�������԰ѱ���δpush�ķֲ��ύ��ʷ�����ֱ�ߣ�
$ git rebase

- rebase��Ŀ����ʹ�������ڲ鿴��ʷ�ύ�ı仯ʱ�����ף���Ϊ�ֲ���ύ��Ҫ�����Աȡ�

# ��ǩ����

## ������ǩ

- ����git tag <tagname>�����½�һ����ǩ��Ĭ��ΪHEAD��Ҳ����ָ��һ��commit id��

- ����git tag -a <tagname> -m "blablabla..."����ָ����ǩ��Ϣ��

- ����git tag���Բ鿴���б�ǩ��


- ������git show <tagname>�鿴��ǩ��Ϣ��

## ������ǩ

- ����git push origin <tagname>��������һ�����ر�ǩ��

- ����git push origin --tags��������ȫ��δ���͹��ı��ر�ǩ��

- ����git tag -d <tagname>����ɾ��һ�����ر�ǩ��

- ����git push origin :refs/tags/<tagname>����ɾ��һ��Զ�̱�ǩ��


