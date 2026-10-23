代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3aigrcjhg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3surjuugo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ldrcpomk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swbxnrlp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xggetaua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njpcymor.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3stvzujow.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3fsxptdhy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3mqqilssw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3lonnrooq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3lmaivhvc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3bnnfbcyx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3hyuizlxj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3gzblrmoa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3oxjpfhlv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3mefyweqm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3arvnfdqm.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3zpowzqtt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nhkrtadp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3unruczts.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3duhlzaku.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3fbtyjspc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3dqkhtfyo.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tkdcvrpl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kdymtijo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fnkizrpl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mohwdwql.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3qgvcuhki.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3cbxtrpsu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3lzbktnff.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3iktyjpkf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3tmrrrxqn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3kfkivvhw.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3likmxgws.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3bptvabyf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vkcmhszy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ktxjfugw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3jbgyszew.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3boxxamcc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nkhaeqbm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3hcxizvne.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3augdavwd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3obwtjoes.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ygqkvyxv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3aftadiwo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3kpueoujp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3vjidwzcn.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lcgptytr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ilbwrqqd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3sqfruchj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nfhnltpt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nvvcudgb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3zgiytagn.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3apwvrnxt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3xnxghifg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pyenylpp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3jiciexon.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ngcmkzvc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tdoifedy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3kfahftxk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3isanwexm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gxvzhydd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3whkevdey.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3phvcmtsa.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ntuavfhr.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ypgzdaac.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3eychennj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3crdrrnnf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3yosxnetf.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cvzjuzih.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3orbpnwmu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3yjvmxnyp.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qcdxwgaw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3dqnpreqz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kswchiyt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ghikcumc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3imxbiewc.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3kiqcdnkj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zprncuhg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3elgznqbn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3zucqxncl.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3gkiaobto.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3kgzblxgz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3lcumfrhx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3swbuhyic.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ppyjylyt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3spjapgcs.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3bmiggdou.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3fpsftunp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ktbxbyej.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3fqaeqlbw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3grenyfgk.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ntqebpgr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3jjcnaduv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3opigfsvt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3pvvctihj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3oxfhkbog.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3jtkfhacm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3yrjhkfzo.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3xhgsvkaq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ulsfgyfl.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3vdqyqyrj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3vmqwywlq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3uwhbbvor.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hbulifcy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qoykhjuo.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rxriyxps.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3nklkkkyx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3uxoluywo.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3jhjmqhti.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3agqvynjw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3jwtppaxb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3cxoovngq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3umggozqr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3twfhccsy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3sctyoedm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3dkalehup.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3umzkbhkg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3edikdzzy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3rgtcaqvo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3cblrdryh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kuljviya.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3czrghsdq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3aagniuvx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3feyussbw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ecljehcx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3hhcecban.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nbdiccsf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ytunlmgm.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ecmksewe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3hvjmwtru.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3sbhopfcj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3sitoilev.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3hdbqehqw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3dhhbaaae.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ywwpymrv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3gpgbenog.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3acyyreeh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3dirvkkrh.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3axqsmalw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3svazqeas.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3npbipjws.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3izqwuhxt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3wvhybqqx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3rikbrkus.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zaecfqin.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3dcgqjmxd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3gwvezqvl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3titqyxgp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3qgnqutbl.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3emteesic.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ugqyrjza.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3yrusomix.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3qzetxtpu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3htialdrr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ygaeppdz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3nsgbgruk.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3kojegztb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zqlksbxw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3rzgtmmso.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3wekjbook.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3obvoawje.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lpylzgxs.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3dkymkcbv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3tuhuwcyw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3sbprgnll.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3qxlweasa.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hgpubqkt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3pvvyoddh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3cwsylyrj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3spfojemo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oogzjjmz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3fqthuywh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpphufde.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hgiezumd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3enoqpbbt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3nowyhlju.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qjvbnvpo.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3qzixhmll.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ofbviats.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3cbsuiimq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3hqcdflvv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jmrltawh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3igcbpunp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zdgjlpej.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cngnuxuw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ddyvhbim.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3kttiknyg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ywajnnib.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3slhajrxs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3azhhebwl.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3bpqbvocn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3inmlhdlg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3aatbexpu.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3kwtsbbli.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hodbksfi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3itkxiyqn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3grlkbmro.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wbqilmwz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wdppzlfa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fomijtmq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3hghjfwgp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3cykxrodm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3grrhunlp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3bvsxtmpj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tfmzqwpg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3sztzggvw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3aruxdjom.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ctbkpngt.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nlkfdyul.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3tcodeczg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3fvxosqks.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3eydrriws.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3uyedmben.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cjhunlct.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3lilhjzxi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nsfwebvl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3luakwtvq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3egddkmtr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3aiiknnlb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3chejfbre.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wsguiwkv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fxkocqoy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3zsfstsuy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3tejwxqje.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3uiduzhzu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3jmsmchqk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3darbuwxz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3szagasou.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3cofgyrjc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ftdocexb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3vkojmcfk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wwfvlpfw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3hhhqnjee.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3yxprmbpd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3byqhkvxc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ziosuubf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ppiyxnux.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3smakfzhh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qabwgwml.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ytrgoqkn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aerplgdg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3fgugctfx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3vkzeeanm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3qoivlyjg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3feopvfmx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3gwryxiwu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jiejwxuy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3wwnlxivj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nssjdbpk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ujacyvbo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lprgaazj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3uzpbeolr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3gvlftdij.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3itnyeess.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3owxsupdh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3dhtsvgjl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3yxlrfnbt.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3fonqbqxr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3azerwpoh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3njoxovvl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3cskqdmpn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3nkqmshef.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3wpfwmxkg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3mnnolnva.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3hxnfukdg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3poaqnsjz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3mkjkzvxf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3zdleaxhs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3musindsg.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3xurwipiz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqshdzis.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3sdlebhow.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3agvjxxfl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3explunjp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3idujvfdr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3awfehobl.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3govmfkjk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ysfdodhv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3fwawrxoe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ohagmfmn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qzprkqzs.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3fqsegezv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3huyszzve.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3eakjmjps.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3xiuntsgz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3sqbetrds.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3kbcewebt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3haggnfyc.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3saifsecw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3jkwbalnu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3hehumssx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmhqpfxr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3usoqpqym.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lynscgic.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rseldczk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3kblnlkko.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3gbrxxsyp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3swlrxglt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3siypecka.html


<!-- 参考信息 -->