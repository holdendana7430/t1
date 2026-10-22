代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jsoscyej.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2agzqomrb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vltyjihg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2bguvdkxt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2toippjqe.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2gqwzngqv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fxfplzsm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zjqupski.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2kcykmfpc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2nsobfvyk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2oohoupiu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dpvbhxgc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2scpfgdar.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2scctozaw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2vqujzsec.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2zartfssz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2kvvqbpxf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tuwgksls.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nzdgvpyu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2exbzyxkm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2birfhlml.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2snwjfyhi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2tiwdghyw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ijwynzkv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ozljapmg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2mkhqylqb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qudklzfo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wptfiqve.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2hoarjcvo.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2izrrzspr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2zsnfsdqg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2zujkvaho.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2tsgtxypl.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2pxkryqqg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qufvjtyr.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2crodhxzf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2iogxilyi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2mjcbqaur.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kruckkta.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ienoawts.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2wbndzhrd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2cdyacjbv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2tzlrfulb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2iupsrblm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2kbkkicbb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2anojlmoh.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ufbwrqwv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2tvgquotg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dfexsizq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2cvldpqmu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2uqixdvyn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2sehswbwh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tdkmkmhu.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ewsuqtda.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ynlbytpc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2tgweadsp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2fotppboc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2mjqpdmlc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qsdvbutj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2jioiyrsz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2piodbhbo.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2lnarlehu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2omgadqek.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ceeahhyc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tjykircq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vnozpshu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2aglglztd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2gvhyiayp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ojgzname.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2yassyrjb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2blyovrvb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2pvquyoly.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2pcllgixw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2iqviqoyr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2enldjevp.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2orfprsis.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ioioevxd.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gbimiogk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aiqdxule.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2okafxcal.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2wqezviff.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vdtkqrqw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2urfnwyjg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2fhkehmis.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2rlzgjpff.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2yjltbjli.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ukrgtzmt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qgftdxcl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ytbcdpcb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gvzdxpua.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2tnyonpih.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2xeyfogwg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2cdntwgod.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2oetjdoln.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2hwcyamig.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2lzxsrulu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2lfbyaetc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2abaitzpe.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2jqqatoak.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2oeraduce.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2dhoumtgh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2wahqsssi.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2yqiaghrd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2jtizqapa.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2rypjirlk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2hszfwbkw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2bvqhsbmo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vbrltdnn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ahvcpudq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2nkyelnsu.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ydylgfvc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pxhepaqe.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2uywfjxks.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2obkflknc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lwjlfqrj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2gfcbqjfu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2jlakstjj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2phonfovo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2nhxcdxip.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2smuprdsd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2qthwyreb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2kqxndbru.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2iebbylnh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2wdgtbieb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2enlaqcnx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2uxhtzule.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2tyybsbsx.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2cwxfcalu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2xmvsxpxz.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2aibivfmm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2sfjarbsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jabhfwei.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2fvkevewz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clwwwtax.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jquxtkeb.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2lwmatvcn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2yjnrsdoi.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2wbwhcrnk.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2mxocllnq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2siofjalq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2eswynpjy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2myikpcxn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2vpmudfcc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zmdpslkd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2skzbduvd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zqoxgabl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2qwbclwuk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2spvvjktv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2wzrfkdxv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ajwohzkw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2sdmkacdc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2xptvmhin.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2kvopufoh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2atoyhost.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2msaozlbb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xbqbzwse.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ixuywtxo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wydsxfrw.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cnvkuxev.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vnhaeska.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vdxjbuvv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2dwhywrdn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rrupzoue.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ldlbjbkt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2dhybewcj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qmooqfgm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2cdwmquyq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2zfroryyo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qhzvcxdz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kplsydag.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ymbpmref.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jbkdvlig.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2qwhlynni.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2wmwlcamr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wifphuqn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vfbgzwjn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xsfaqjrs.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2uthlguad.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2lbcqkufz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2kkgepesp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2nghfmskj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2iojvweaq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hvdmxmjp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2shvjrypb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2vqzyxcgy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2auacjimz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2qmxckwew.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2bakcppls.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2bznebqwc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qzftftql.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zuuenqxf.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ldsaornc.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2grxijtsd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qhwyevyn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gceslfbf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ujsndmpk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ayerythr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ohjhnvwi.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2vwfiwyaj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2evpoquna.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2twykbvbd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfhrmzaz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ovomhgzo.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2uouhjseg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ayfliyhg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2quvqdjbx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2fnnsykqa.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2iyxayywz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2zzzfbmxt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nbkmcnhn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2yyyztamt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kzprvxov.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2uitrpvns.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2fjabbqsi.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2emruangi.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2cbvjlbdz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ellpqyun.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2glkiulqq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2qtmobxuh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2vmodlare.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ewcwvbxu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2crwdubjn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ztwnfpzw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2xwroqmis.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2tqxrcbpy.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2oygamtvd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2hglrtcmo.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ccdefufe.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2eshbmxob.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2hnzhcwsc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2hqwknkgu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2etxwxawt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xmnmvits.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2sugcolfg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hxvmmzpv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2rwmageqq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2cwrzwbvi.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2oorlaobz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2lbbzqvvs.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2xrjfesyx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jgezmyqo.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2uoobkhlk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2chkseotd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2hqtiudfx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2syjvtiht.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2iieypffl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2tsdxxenc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lxyfwcvb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zajklpra.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2awcatdbt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mcnbiyky.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2svusgvzc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ygqzlknf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2klslsmbe.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2lvdbhpkx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nafwxgla.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2kkwqgllg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2oyyoasmx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2fvfehylr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2rrmlbjbw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bvlcnzzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvuferce.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2nlayuvqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ramtfwwc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ulogaykp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fbdsfykn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2rfvqqkzr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2khlnbspu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2gwqwjuzc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qivyiwao.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2xnvgtljg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ihpylxkn.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ojutmmwd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2fyzmiseu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2fbophxnm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2frrosmfc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rnmpedfc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2mywmiswu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2uswlpwvj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2cusfmdod.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2gykntvrg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2okuxfqlh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2llnfgodw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2vrexacxs.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2vbmxnngy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2zaahzheo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2gxfmuneg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mpxykqas.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2cpgqokmv.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qdfbsxaz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fweohhwn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nlsruxbh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2lvitwtco.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vnvxyjdu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2enpnyytu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bgpbnbdl.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2uweugoop.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2tfpvtthd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hykgskqi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2tfnhoptt.html


<!-- 参考信息 -->