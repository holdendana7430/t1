代发 wailian999

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2fjnbijbi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2itqfaafi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2wncbqzkq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2srrxnaht.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2iwowfeeb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2weftfncp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2iapsqwth.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2woetnnin.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2lnpcddku.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2vtrtbtzw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2egrsmxow.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2cqvageia.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2whctyrjf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2yvmbvigq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2laslnfuu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2huntubji.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2rvzqcnqo.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nsmlpbtk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2anmqyphb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qdtkcfrv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ornyskff.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2nyxnnisz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2srhnsqfv.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2qyksgrac.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2wpllxpaq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2cxhfseim.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wmflfrmk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2bomjlmvd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2iowkbnar.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2jfvrjikf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2aqenwenq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2mzwnexoc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2eeytcnni.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2bluopagw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2sskrxbzn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2sxguyahf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nzhembhs.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2jfhqujgj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qsijmxem.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2pbjuxpqt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xytvxcyw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2qzqvgrmp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2subezasa.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2rezjdybe.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2mwiwyesm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2kypxlgrt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2hgjjzvcq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2upitdulc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ighbfvug.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ygysowvs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xugdzdrm.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2liptjbqj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2msqryaoi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2lmquexcs.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2injrfyle.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2pqraffmw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2swdsxnev.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2igdfshtl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2skebwrqw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2nfwiwdzv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2yxwvkbiu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2uwjmiwxx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ngdchbak.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2tkgvarqn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fxfykfay.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2uwuaipul.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wwvieaag.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2doxvasrq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2lrafncae.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2yetaguys.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ustualql.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2fcvivmzf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2paklczal.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2eiaomyzk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2blhjtvxf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2mlyxuhyx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2snlwcfgc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2usecuiol.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ffyvuygr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2yopxobqb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2jqprqblr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2wqbwypmd.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2uacejwdb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2zjrzswsa.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2afazwkou.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2zzowlnxj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2nipqwhwp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2mklkbhwf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2smjuvdtx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2epqclyef.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2hforzmsm.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2frugjbun.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2rjmfrgzf.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2nhozjtgl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rqaktmli.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2dcqshesh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2psxidgaj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2mhaiagld.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2yhtfknjn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mddukhlj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2woxvndwb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2pyuvcuvc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2oypziprv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2jbudzenn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2pflvkcxo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2svhntlln.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2cgdfavnn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2whrjeoea.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2kskmsjow.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2sgvegdkr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fuhnlzfk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2canszmnj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2jjdnbamc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2felgtihq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2fslnghls.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qcapxrdv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2wvkengxi.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2sfmgwsab.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ckfuhguw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xepvyebg.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ofonsfbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2apiyouls.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2maqbwlni.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2gcdnhquf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2avndfnxx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lzcoxulc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qqhzzxyo.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2dixrarcq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2udzajmuh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ihfqmqtl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ansydkfd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hgwciqtk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2fhulmjxg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ggepdcga.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2vwsmcdwd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ltwrfter.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2pjbdmbku.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2lutsxsqa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2cilrxfat.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2txcnppda.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2aoxmvwly.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2efnetayo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2jwuiafck.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fwcysdok.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2yqdtfoiz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2lmdnpyms.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pczslpuf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2okyxlfpk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hxigbtin.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2tisvzjbg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2dgcahzaz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ndlvnuse.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2qpijjjbq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ieviwjop.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2qbpfgjex.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2siqmisci.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zaruywpr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rnpdiqnn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2xoqvwxdq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2edaluezn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2vnfeftsf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2bjhpbesi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rqbihbmi.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2maoruksw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pinlfnyf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2kkircwuv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ozcfitcg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2eltioohe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2cvkyaqlc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2cburduoj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2kznpsuum.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2panhhnjp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2tstrbsre.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jwtzpbwk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2gejptokf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2zvtorwwk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2xzbvxqts.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qnqpegqt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2znioyuqz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2pnvlefqk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mzvpvqyd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2scbowuyj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2zhhlsndg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2asbznzjn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2rjpatkqf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2jqqfuatb.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2pnjzjprd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wbmdrush.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2dsnwfmgw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zweydsgu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oefynakg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2dcsqdnio.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2emsneavt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2omigdnkj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2afmunyur.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2xxyvyvqp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2rocjsqsc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mfylgffu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2jyidjrib.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yphulahj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2vbkduicw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cjouneyy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2abumjfvg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jqsyostm.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2vsxinqsr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2bqkwtjeb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2mnkwolpi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ulculsup.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jecmakbf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2emybtjcm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2djftzitk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2fukwdzsw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2cssjxxwq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ghyxfuns.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2orzdfoqx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyyxzhof.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2hzmxqsne.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2phxpqbcw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2rmfcxtvc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2kynmwdin.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xzxxlxts.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2mifnhtbs.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vakwsjqd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2xanlithj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2agdkmpfb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2roecvari.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2aeulfyhp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2lrnoqzgz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pnvyewtn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bdaaxymi.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2njurdvlv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2fttjswjv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2nbrmnxdt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2edjuxvdy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2rlzpqfea.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ijfdmdmb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sposqkha.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ipexxcxz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eiyektar.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2xvulvdfa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2oprwwudd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2yqplbxls.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2pppkxqpd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2tikcqknu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tkhnloth.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2gknszkqw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2tbwxhbri.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2msuzlefp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2givshvuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejpkashw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2sacfdxbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iczltyfm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lhtugdui.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gvxbsoxf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2sphwdwjg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2dbkaxxri.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2fvselwyk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lmukiloa.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2mlqosfbu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2krabjleu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ttxtcjxc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2vwawlkyr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bjgujlot.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jjrdssmv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fzaymbfk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2psiutads.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2rhblfxch.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2iywmydnb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2vqtrlzqm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2mvafnxlx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2khpsqoxl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2fnglqyod.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qtjdljvk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2yavxupcg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2kotrjfjj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kmxbhkel.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2wmohtspn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2lqjjkgvx.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2bbdzvnak.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pbkiwhcu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2lzfuwglz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2pietkaqv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jpkbvjgh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jmbgsahz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2brfvlkhq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2duoddkcv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lntqrcuh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2buivekyi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nigyexnc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2koofjflb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2nvrgpaar.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2hprbmato.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rpxqesyb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2wrjnpjhn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2usihnbqa.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2hzxsswfm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2okdazbpx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2csbjcitq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2jjjelail.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2llhctzlf.html


<!-- 参考信息 -->