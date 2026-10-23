代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gdrdrufe.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3mzrorhtm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3tnathhmu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3olebguxv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nhjqxarv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3oryvhxxj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3hptflnqj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gftacmed.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3gxcivlfs.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3izbppwhn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3fgzjnrvz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tkeqpjps.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3gwvkjaef.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3oldszwpg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gzjxhofj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3eqoqvyav.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3bghzeuwu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3bwagqiym.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ozeokcle.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3uszzuovi.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nymwzmxg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ghcongab.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3cqgpxdcu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3nerszjrr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3nkzxgfrt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3woatduve.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3spyathlc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3jydgfoba.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pddowcbo.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qufwtjiz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wajinihj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3mrkmnkkq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3abtxipus.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3rbsykjgf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3bvkfxijg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3abwbvgjh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3odtxxxrc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3cnulzrdk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3bfrlrafd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3yirfuilf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zstlvnzp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3yjiharza.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3smscwhnx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3gtkrpdpi.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jolyyjzc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3sqflljjr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3oirukapy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3egywbast.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3osnovmnr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3oipsdykj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3azopyngk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3jkguusvn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3stdcnepg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ajwezmzw.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3cjodymlz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3wlfpdkxv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3vwhytidm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3pnksfvmz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3wlxpjftu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3mzwofnll.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gnpyeaaa.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jedfllzd.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oteozbgu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3exxcjjns.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3bhumufcj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wmncrvke.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vjmsxclj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ltrcsbfr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3wjchdnsg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3mkwcuqns.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3vtivtxjw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3fnretlwz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3uygrwbao.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3uyytyyoi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3xnolneha.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3qdslwdtp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3qpnxwftm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dfzpugdv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3zraocxaf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3lometwpb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3dhuwdtme.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ugscwyoj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3afnroxll.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sphcwcpg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3vzoquxwm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hpzjuvrw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3petgccsk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3kzyqecns.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3nqansnkn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3oretrbsc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3aobnrdhf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3pkacjgmn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3iqlbqynj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3xwhmydyb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3mbbchnum.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3yucfjfkf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ymwrnksm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xpuzmwro.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ogukkwaj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3aranlryc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3eidaveyi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3irbworcn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nmzqdeqq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3axrowgwd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3nxhvkmph.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3aeklctgc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3unuebgbj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3waakwwtv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3nbhbfkha.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3tesdvuae.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cowlxeus.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3wcumrdij.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3nkaqtlln.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3elzcaejp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3qzqoisvk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fbjbizli.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ukbxcfgq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3dklhuooz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hocucwcg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3wmamgtlz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3aicvitwr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ykvqqtbj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3tixkwjmg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3qllfbhdn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3exhnqmsh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3kynbqdys.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3asmsgqwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjmvzphe.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kbgiaoyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htynnjyw.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mtubxfpw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3zfmhsxwt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hglutatl.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3iokfnlul.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3lpveluly.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3fxoextbd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3xdupnscg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3lokxhmnk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lbydocuz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zfhqjvhf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3qrllbjku.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zejmmzzx.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3xvjymmev.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3lxymenin.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qjebdzzc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ysrmfesh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3dojxnzcv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xbrkmzdp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vblkxdkh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3gscjxmyk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3tnkwbopw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3msbkzjlu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qkrutadx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3scucpycn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jbiisrma.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3tjugsmuj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vsdobxcp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3nbffeqaj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3otpmjbvy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kyuwncad.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3yvyxjzrv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ynunzpch.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fnkdliwv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xdmjdguw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3hxznroqk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sgerytww.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3mxfsagle.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xwbspyzi.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3tayxolln.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3qcdllaku.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bwxuoabo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3idnurhvj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3amezpapg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3buaxjlmr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3oxktxzmf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3jcnqjcnj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3bfbdueeo.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ciyhlgkp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ynevjgsz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3bqgbufvu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3zzzemxix.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jevpfipz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3qwlaokxm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ldmiabsq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3jmvhsnwf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3vcmfeudh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rtzuvtmc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ygzbgocs.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3bonxdulo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3iysqgwtk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3sixzkbmy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3igsqbkim.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ukzpeqez.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3taaxcjai.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3raqezwaj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dwbiwuyu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3oqigkivo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3senqtnwh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3usxicadh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ptdgtcja.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3maxbztee.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3czjwbzmm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qaccgfoy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3myqwavpa.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3eigythhg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ktyhhdbo.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xmyakdkr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xmpvtiao.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ygigxord.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hnfbebzu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3utnkmzib.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dootkdex.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ooiznytn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hpqqjpdl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3lbzgmwhw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jxtvxohf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wbtpvuno.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3selhymbo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3tqciiekj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3wcpiztnb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3rolfxeed.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ergkmcqy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3mzfzweec.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3lhfmvxtk.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ldjgbtwn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wjgebrbu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ovrdypyj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3abdqkolf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3detybdsk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3vhehfeby.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fqbbcyab.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ugiguggw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3rzmbeycg.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3asdqxmax.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cvwwhzgj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3nhcgbtoz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qafsumgw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3oknakcgr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3tbyrslkp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bstlagzn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3qevyuwpc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3mqqgdszq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3nisnixnk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3tlbkhhmq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jjfquksr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3fspmdxtb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hhobnuia.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3okbsnyzd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3slkjavxc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3hduxwbhr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3bsoqazqa.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3drdvjtix.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3skszbykv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3pjbyryof.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ouyxlryq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3keyzqnrh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ukfuacyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phsxngpu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vlsrhrmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqqgoart.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kwzpykuv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3celorfbm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3qzxynqba.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3oaimwzmi.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wsjtjvwu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3roernpma.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3lfylyqrf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3woubrnuk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mjohpfzs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3tjwsyiwz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ijxybwbu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lmbncqzw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uvsfmwna.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3weurqelq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rvkhjnli.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lawzrjme.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ypfqyvfn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3adiljnyy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rbgbcqbg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xascbqbe.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3rrjfkfkc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3bejuqiqf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3wejjqqzw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bpijjtvj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3uhtqzvcg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3klaukaiy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3symgcxqp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3sgpydmfd.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3qbyilxdz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3muyruuzp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dmuypjkr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vohlqvdf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3frqbbbky.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cskcmbtw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ebabdvoj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ilddnnwo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wmbavifq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3llpwomtn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3jfoftits.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bhzeiidx.html


<!-- 参考信息 -->