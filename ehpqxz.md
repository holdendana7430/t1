代发 wailian999

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3lewxxqgx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3axptiroq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3omjmuylz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3eyafgyig.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3kwhfegdq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vripukpd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3lxtbaoar.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3affgvoro.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3piitoezb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3giipktnh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3iexdhkje.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3bzthtyug.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3pgdninmr.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3jszblvjr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3hfpvzonn.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3wrvfcvam.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3cikmjjci.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ukcnlqjn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3izqdewtx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tlmwwmos.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3nzannwwt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ptonhxio.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wlcmhzme.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3osixumig.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3pvbmytac.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3kvqtgikm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3owgiizfh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3xgvoebdr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3msrcxvdr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3yxpjoquv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zvcvchhv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3plvhjmky.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3kqlbnbjw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3cssundrf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3icpcsobr.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3lfebtemx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3quhvsorg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3rfarnsma.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3kcjqhjkn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3fpddimmz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qpwkmquh.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3gluhgejx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3gpahbdxe.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3mbabyjpc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3eyarwnbh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3uplzseat.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yyufwnal.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3sspywxuc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ohmjgtaz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3uflqyzea.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3cqikskkt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3essttskw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3syocnggp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3aicsdwxg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3vwesnuxq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3mzduxhph.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tkuhozsv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3asaeuaiq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3exwbjuht.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3sntevdof.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3qepxlsiw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ydakyqgh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ifbpheyr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3lxmqluab.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ibzqhfiy.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3hnavjmoo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zfoigrpk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xbertlhm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ahabeduq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3fmnkqtfp.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3clmljbgu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3xuklfmjs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3wmctooin.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hdunveid.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3wvgyftde.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ibbpdiwb.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3foeueemq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ytnsewkj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3esyuogtc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3iapgggvp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3qbskwgpt.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vrervqov.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3jzuvbfpv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3fmejxlfq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ksqxnqbt.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3xayckopb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3zmauluwc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3wlmgcshx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3fqniyiqv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3aijqhoyf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3btlwnwth.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3wxletrou.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3malkewez.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3abkzzppb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ccndsiif.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qrathjkj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3rbhhynau.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3tsegjneb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zuccvxln.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3lryzhpbi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3gdjofyrj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3phspbvfq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3asbwutlg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wvcxaumx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3uqlwzonk.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3smrvzeaa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3oabeitho.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jxcdevuk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zqgettxd.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3xosjcdnd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3grnkujfv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3jfwszsyd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3xxgwkvge.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3shgnhmaz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bqcubpej.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3dqwvjeon.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3fsbxzefb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3gmrbslhx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3elmfulcn.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3dhogszno.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3yozjenqv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3gbbyovhy.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3zexyxihn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3feavycdj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3lgepwscd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xszrjhmc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3edbmtrgf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ndpixzsg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrmvakxp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xrqbuxwj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3qgpwjykv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3flqeosge.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ltjnowlj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ymxjamgo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3hhzqfajz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3udlwmcon.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3atcsbmgq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wsbubotw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3hhfxagsp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3dikwghaw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3dnelqgky.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3nvhcxmmk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3eiftraca.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3htkooppb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3oaqfnfmw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3xtpkxrfn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3bpieojmk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ybqjpwuu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3dvqddcjc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ckplrfve.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xpuxxtjw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vwiwifzk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bxzxpkob.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3cwoobclv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3zwlbduro.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3umugrlhf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3kpiirubk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fmpunzct.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zfenmiji.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3rmkzsjoe.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cgzndrkh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jnfcjxtn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3fkiypziv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bkzzcoyr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3zyxyhyeo.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3uzyjpbmf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pwwknldw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3dxzuknfr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wbmgfoql.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ygjhxych.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3csyklxul.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ohmsmand.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3sbdipmrv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ierhedzu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3aytzgaih.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3npqqoppg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3klqpwwme.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cqsinhnd.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3gvxltpgs.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3oejjsfoc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3gsjgrvmr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3bfgierke.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nsbgwrqu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3tkjpthfd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ckcmejkw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3qfsvrfwk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3tokrutil.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3udynmycc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rjlvfxxm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3upefriqb.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3soyiynht.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3atnniveo.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3focjruzr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipsbugcu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3xatwquvb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3hrhgwfwb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3utnedhcv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3rlxksomj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ekknarax.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3pdyiphts.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3fhlvrokz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iefzsezi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ccmqhgtn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bwntsiuw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3yybiiqzr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ramwisoh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3plclirdu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3drwkttei.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3mrlxvcdt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3zuvdmcgo.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3aefhmdtj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lgrwzatn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qtksboeg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3kimkcgec.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3gizekvlp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3koqyoesx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3larnjbsd.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3tybtwofj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3zkvwteev.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3znnawpsz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3yqpvkcle.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3cakmxykz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3mmalmcgw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3rduzahgw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dzmhtnvf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3klhbkwxy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pkjikuth.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qxvidpdu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hfevxkat.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ghwvuufr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3uudnlnij.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3abquorei.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ysrubhjz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3oyygqafy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3jczlkran.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3nmljcwvk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3hnbxevrd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3yvskobad.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3mznmrrtu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ddvjevaq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3bjdqjmsn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3axcczpgc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3hospsgyy.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ewpquqwm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3pjksmwso.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3vvxbffac.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3mvttprbu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3nspshdek.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vtlmkfwz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3zyalvyjw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3mumamatd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kacbmbhy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3urftjltj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fxkikxrw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vqeflcdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxeltgbu.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cvtltnot.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ikujgypz.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3oakcwmpi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3fkgdccny.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ljhuhhge.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xdkstrer.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ietuqtsp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3cbvtkplc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3eiuosxzt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ewkfxkii.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ytksklos.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yxntobrz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vogioktd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3tbsmgqdj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mzkqgxej.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3asgoykgt.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3qluuryjn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3taktfjqq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3uefefppw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3somckfhe.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3phrgvxkp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3wdvgirws.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3roeaakxr.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3asuxhuaz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3kenthbam.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zpybgumd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3iiwavtci.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ehqxzjby.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3gvrkxaxz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ynwfhvls.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ptncpqro.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wlxtsapw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ezkiqpkt.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3wkhpbncj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kxotbvue.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3jeofnehu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3dipsuivg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3etsmxtuf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3sgcaagms.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zrhlzdim.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vyduapju.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ummtkgxm.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3aghqnkmg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zclzotgw.html


<!-- 参考信息 -->