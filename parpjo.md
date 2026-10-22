代发 wailian999

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2oyhntihg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjwkqgsq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2qqrsszeu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2mtucwmmf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2lzveaurb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2kgigupik.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2qilmzyhe.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2iocymlmy.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2aokyvktn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2zcolvyza.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2cxgaapya.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2lozkqoli.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2qwikntpp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2aatypxav.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdvtmpjm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hntvsaar.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iyqejszn.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2suizzjiv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2biobpcmr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2swvoleze.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2fliyeuzd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2yrmkyzty.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2tsabbipu.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2qssnqfvc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2fwpiyxjf.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2qkdjciof.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gvzbrrxw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bqxdsgtk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2vvyaspue.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2xgkkzfvl.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iqdsnrnc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wcavnyez.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rfpklzdl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2jmkklwke.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kjehraqt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cvohnmcr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yhkrxrbl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qdaenpmt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2djkacafv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2npefzsph.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2wmihkzeg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2dquexwtn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2swidlkjr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xlwhiukl.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2xwlwxxjj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2wyfoocmm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xbcblzrk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dftweczq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2upuyjbxa.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rjsrpegc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jpzprput.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2advhmlht.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2maemmpdo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wdhnfzct.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ugobfvgh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2bzknvjat.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2yxtxjwcg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2yrsycasd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jevzlysq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2vdprpwid.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2dfmxentf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2wsqdfyzy.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2pruauujf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2urafkjmq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ooareqkm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2daohjycy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2sqdxbjxw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2uurnqqlw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbzaqicg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2arzqqsgq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jtohsjmc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ielwljjy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2depllsvi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2fbktlfaf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mzcmnjmh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jpxkwdmk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2bnnlwifp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2jyjjqlbl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2cvkuqcmd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2mlcdnthw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2iswtnlue.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2khwzthjr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jzbexwgi.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2qrckssaf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hujxsmwd.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jzvlpghg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2zbqstsbd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ahefyumx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2sicrfeds.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2juaqyvvt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aajnglmb.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ndndzqei.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2okrwjtks.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2fougexgb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rtjbdaca.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2adyvuxnk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2dtmjrpqj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2hgdykkyz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2liuzrsft.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2fablvoyr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hzsixtax.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2vzmhlodf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ypnfesqo.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2lgggfttf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2fboigzpz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2btdjatbv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tennipbx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2fgztjwnc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2wtqcodjc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ydifsxov.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2eoswgcgw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2qalzrlkp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2muzcdgpb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ireqlgds.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zhqbbhhm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2vofoleuu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ojhrrooi.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2oszkitdd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2elxyvutg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2kqpxegju.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2cshvlyuz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2uqkleeca.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2jnphdnsn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ecruaktc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ghvwqxzg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hzjlunkg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2nqsgihxn.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2xifoifer.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2hgphdubb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2gvyrfqnu.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2vmfrhoji.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2inexgizj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2plpovghf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2sybrktmm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2xjimlwnk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2odprbetd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2jvbgrkby.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2oelbudut.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ltadcfbx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2bruhikau.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2gtruqspt.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2yxoljwdi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2kuzeurkx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2fvujkcne.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2omoqtvli.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2wamwviqy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2fcxcvfzc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rvzwaujn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2zndmjeuh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2jjpzniva.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hanxaawd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2njnpidsl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2jijneicd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2xbeqkwkg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2vgfvwgoo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bjnbcehg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2efjtnxpj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2nxxeifyn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2teguypng.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2cqkdjeqn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2vjtwxiam.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2zqjhgxsc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2tuqtvqnz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2bmjvjzvv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2rpmgwjnx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2wyopvcih.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2dtbgppjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dixprqji.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dcrmtdtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lsqeteaz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tfwzfftm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2bshzwqve.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2anpppqlz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2kthdoliz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qeogfqba.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2hkdfwzxa.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2fupkdrge.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2vabxglsa.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2skhjbmlv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ykyhkhwl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2rrhqsqpc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ifeiivsx.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ahapagum.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ujiemael.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2gejcoorw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ibnrfdfm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xtbupikp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2jeygjfom.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2wnagrmlr.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2juahrjkq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2qsqkobiz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dleqmgnu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2xvbettxu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2pcmjqywp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ggorlnrm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vhwcwacr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ifpsrhye.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2uunwrsdd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2wbpzwpmk.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2zpcxacqx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2bkvbnkpi.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rhfhbdzu.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2veionwxu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2azhitzgz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ujxegmnt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dnexuzdr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2njukioyl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2arkacafq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wxnzajmt.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ocpgmmjz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xcjqeywz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2dejlryij.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pbjltshx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2irzjznfk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2pzsuvjsy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jdoczmgm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2cphoeskq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qrcpjsuy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2vljebqqg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2okhywycq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jpkernon.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dlguibom.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2wxyrxljh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2fspwjfaz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2bzbdyzmg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2hmoumtch.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fxxzvufz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2beosttay.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2fgaaguxt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ozpcfvxa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2xinopdbm.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ysoeugvp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hysnqgah.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rmzxblfw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2sghmzpeu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zlswnlvw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2prmgyfhn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2dpjavvna.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mpkauegj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tdnsvbnw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2iwidckma.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2nuaagknr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2lohwjpru.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmnwzkas.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2zrukvegw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2chsvwgna.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2zmrwmkpd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2shcomgct.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ypqcjxdc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ydmmnfoh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2cuxhtnwv.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kxnwffzy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2vdpzkxib.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2upckaokk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2fciiqwbm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2alsseynu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ygszltsn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2nnaqjnmg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2zvbsfikj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2dutbaczn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2pgeyznok.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2pqcxztio.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ceqjclkr.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2oivgqqav.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2soicvoeq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2yuzvhxss.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2aoqhmwjo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2joaiiwrk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2tzpbiwhj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2rklchfxu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hcthyeoe.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2rhvsdsal.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qqpubpgm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2nbgdbbfn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2juhkgehn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ywkvrbkw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vabtfyio.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ikjvvhrs.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2rfzvxyen.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2qktmbkme.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2xyhstwim.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2lubgzyqh.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2jlyeembh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2pmfcbzwm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ahyqaaqe.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2hbkjgqff.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2iudpdyke.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2hprygodh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2htnlcehn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2jebotwrm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2eksidiai.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ayfrbrin.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2jglibltg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2tunsgpaa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2nkfuymsw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2mqvzcjhq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xttlcntt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qayruspq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mfavrtqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbtojaht.html


<!-- 参考信息 -->