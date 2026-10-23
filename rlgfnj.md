代发 wailian999

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tnqzqgjv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3zgfcvipp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3raoaeztp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jyvpnlts.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3jpirlpnp.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rsdlyhmr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3slkrcaoi.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3cawtvfgi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3dyvssovy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ytbvezsw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3sqdknhlb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3tuighcck.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3xvkcopal.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3mkjluxps.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ngganaob.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3lvqcszst.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3iwmqmzij.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3sdinpnez.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3emadqtrh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qwbxlegc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3fjjkldzp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xgbuqunm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3pkcyhkkz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3iwnlipgy.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3tlaimepg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3qxtzwjnc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdveuqse.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3afflbbyl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3rmqywnic.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3yzorjspa.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dxxjsepf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xehjtibb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3nwtdqqor.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3jpyyosqw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3jfrrfhai.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ukekqdqb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3dcraepee.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3hxbvfefz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3mhgwoqvi.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3caeheyzi.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kogaslwz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3uwikknvi.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3wpokcjdi.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3vxlbzqxb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xgimibvb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ktkgrgfr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3gsnxzrzj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ltslvutj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3oukvhblq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3soqqryxp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mecobqob.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3oqwsqkyw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3jgrqofkt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ogortzhv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3fggdeuuq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3prywtzja.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3udfiibfp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3whuzrfmx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wwitrofr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3njusucfl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3gmxzsige.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3igrnicfq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hlzmvgve.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3rgcbyzwv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3pvgcctvi.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3nwavjied.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cusvlqkr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3awwsjepo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3djwxkfuk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3yvjkthwr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tyyfkdcm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3eaysdyic.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3cksilanx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ikgnctuj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3alxllpwz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3wbafgwgl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3pssnbjgs.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hyyadhaj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3kliduqpc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ahnlpgya.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3fpqlhrwv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3oeblqvqy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3tzorxddc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3imzxbaqv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3orkugpay.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3vpqwkubq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ubmfztsk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3cjtcaucf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3beoxwzkz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3cagttsin.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3uboubhuw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3vojumwsh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3tdftynkn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3oehmhudk.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3skakdqbg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3oawsmcfj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3wjamtggn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qvbjjotg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3lbiighyq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3nbwqetfa.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ojgodtmt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3rowhunvq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3uwahkdzp.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rmftnwuo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ygcitehr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3raxevrke.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xwfdbsax.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3nouwjthh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3rttnudad.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ioqchacm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qooropes.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mpjxvvdj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ibdxqmts.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3wbkntpit.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3klvfnghh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3dcgidrsx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3newelujt.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3pkeritbx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hghanafi.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3oaldnjer.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3hoebvqhq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3zujpdmtc.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3jymlxgsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qcwdhirg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fimtigdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbsizirb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qrqsvzsv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3gqycsigh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3emdqcnnd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3oovvnunq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3xxcecdcl.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3cgimtcib.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3hfimlmsx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3dweahsnh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jklhnwxo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nubsrnoj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kkvfafmt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jiusyies.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3lmcoikto.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3bjduhrjx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gjokhkxp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ejbxroas.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3cfupyphj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3bvmwilfj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3xpdzpgni.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3wavtdwtn.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3efvrnaun.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kukjfjcu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3mbkzlldu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3euikyvqr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3adrthxxd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3qmwzshty.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xbskfmas.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3oaexleny.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3leicepbg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3mxwhslnb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3obqnzauh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3genakjht.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3xqiwenab.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wbkrscaa.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3aymmxlsd.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wxftpqph.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3kgdupbdp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3iscdikpx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3oxnaduue.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3obhbiotz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mdhlrqin.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3kkgbdxjg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3snbbxcxs.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3qxnruocl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qxqwzgck.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3axsehkro.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ziernmwu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fpyyoxjj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3gddpfijo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ubrzagxn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3wqlsmaqc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nzpxwfla.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3onaabcmt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3onevjlzr.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3bfsasafn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ukdyaywb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3neqjtmom.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3vjrxgung.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3gegigmfc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3gwslnncu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3aaqqgglq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3iihwzdkd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3rddxzssa.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3rhevednq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3nnzljokp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mpffxjxd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3mtyetkju.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzzzarrq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fcsypcvr.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3afvkrqjz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3bvyxfyrj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3eyambuci.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3uysdgiwb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3aqutfndr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3poefctol.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lhxwlgdb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3njxmuhns.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mwmrzxut.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3fksrmdoz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3prmahmaf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3idwfxiwe.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3udqjbvan.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ckcrqzib.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3baotjvze.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3bznxoctf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3sbypcliw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3uugyjupl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3mvdtwbue.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3kzhlgcvb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wtyarrcm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ghsxszoj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3banoqtuk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vmomoafj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnujzgve.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jqddvqwb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ffrkuigq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3rvuomhsg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3xjqnbpog.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3bmcbfaec.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3sntmpayk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ugzoczfz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ulnrofpl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3syqzeuro.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3qfdcidjl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3eatuxxfp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ljwjdwlz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bkjwrrke.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tulkuiqx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ltwojzfp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3lvlzdzud.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvdicwei.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3imdtutdr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3fogkwsmf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3hefwwluy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pztxolsk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3spbzbhiy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kknlfkcg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3aatnknth.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3gpcqabhg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3nmkhjiwz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3hwtwwcqd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tspykvhi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ezdiywmk.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3gyvuuawx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3xjzhsxrq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nfqzgbit.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3sspcouox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dkbkyyxd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ndiurggo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ibcemrtp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xcokwevm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ctytftij.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3bggangwa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3lpxuwnok.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3hjlykacg.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yxttwbxe.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bynxjzdm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3wrepczqv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pkmkofqe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3cdqazbut.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zawbqgwj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oybiaecz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3puotzpmh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3rkxgkncq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3fgpqdhje.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nwttoqrh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3idxhqkca.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3sfttkdin.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3xhtzjurd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3pqqcuqkc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3tnbwnxax.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3kwuwnnoc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3neixwrmi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wyfrkwzw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3yidmmvnn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3vanbexhw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3lwtlogiy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3yftxqvvf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3fdiwwahn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3otcyajkv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ylgshpqk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pyszfkux.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3xtnjeuum.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3upfjpzpw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jwtffjag.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3hqlunyhl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3otvtnvuh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ydzmzjyp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3djqgnfmn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3snfaurxr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kmhfekkm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3eaveewny.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3gdlxlfxn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vzniluex.html


<!-- 参考信息 -->