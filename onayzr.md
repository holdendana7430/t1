代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mfiuubwr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ccbidleg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dnvlteat.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2nudwkgoc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2mnimrnls.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2jliwjvmw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2tqscrmfm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zmqfcouh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wfxjlqgr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2nmeazicl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2mxtshqeq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zywxsnyw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2rytedshb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lqfiapzv.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jsuodzrf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jticwowq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2qztilwcq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xllurcul.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vgqgtetd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2uzdytaci.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2nvawronh.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2wrhzirle.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2dynfhbsd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2qqzfgbex.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2sleoyxgt.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2fcofnbbo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vazvppuv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mghurhts.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2uehlgjtr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2yhruajbl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ahoxromk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xqgvdjsn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2uwdidywc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2exofvkyf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccmwnkil.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2zqbqdqnk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2zxricqil.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2bnxkjrwo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2nxxbuicw.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2wohvujvj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2yaaurton.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ggcottip.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2lfivxdlc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2nrhiqlcz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2qzmpmahj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2wqdibtkn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2pnyzdixg.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ovhzacmr.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dglppzgs.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2hbytvkuo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2hqxmqzuq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2tgruhnys.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2olzgrqxg.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2uwbbcqrb.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2xgeqolcx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2vyeirena.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2jjghupxg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2pnmxmlnx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2aanvqrrb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ykipxqbx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2esbcimzf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2lgqxquhf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2liirlxwe.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2yltgguvs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ccjoengd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ehepcnos.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yychzwgn.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2hslisubo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2fjgoiimf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ssfrelpz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2noroxgre.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2sowfdyeq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2vfxwisxx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2kiursswu.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2eizjglzy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2pplhroxq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2sydcykeo.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2bugcxcvf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wnlwwsjy.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2hhqznonz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2cpdtjmae.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2aecsjihz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2uexgdyqz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2xtncdfqo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ptdsbipp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2bilexbbk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2twzdwcfx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ouezujwf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2fiyhkbzp.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bzmpxjjo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ltemyynp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2jrepiegy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2dmonrpiq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2rarbxrfd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2mdcvpnkv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2jvcmmzla.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2halweggh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2doxplvxr.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2esfbosvy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2goohhian.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2hbhvjwgf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2twscznqe.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2jdjwnrlz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2qdmahpql.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2cgjkeayd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2uffxwlrh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2unodgxll.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2tgzrydlt.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2bmfppebm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2cjkawgdf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2mpxquras.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sxdjctqz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2qwmpeids.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2zutfkqox.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yzxmcaoy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2vyvetosm.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2nwolxccy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2dnnafvuf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ofgtuqgm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lcfwadlc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2pekkrtpr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2jwausreb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2llxthsoa.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2yxudilsl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ircbgogx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2jmtjxkbj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zwmtzqwu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2sidpymdr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2peuuwslf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2rflqnkvg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2onesdlmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzfvhnnm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2hovibrqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vylcbvzo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ilqsspti.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2tigjdxhx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2igalleic.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zkhwbece.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2adunmhji.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2goymrqto.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2pqqmqygu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2nxcukfjs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2nqrkjgoy.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2eaqhjwfd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2awcywtxh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fonuirrq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2szoetwos.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2dlqyaeew.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2lydytfvu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ldkbhaae.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2igihspdd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2domqoctb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zipgziiw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2dprrkbsz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zxypppcr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lgraekkm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2texnayzz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2kycuhhsb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kztqngdd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2aoipbwyz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2cvxtqmzo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2spknfxnp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2uvczboza.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2bkpfilfv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ncrtqwhn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2xbgzzuca.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2dcrorvsg.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2paejfiwr.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2itywouce.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2teqsqxvz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2okbtmbkr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gptczrar.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2wdmprrjl.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ctssmtfg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hvamxkny.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2tmkvgedk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ddukmczv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2cyhwqhfm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2qopehnek.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2eutvouxa.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2rwbluzqj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dnehibrx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dcxbnpla.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2jctawymj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2gatpzaoq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ebkqptlu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2txpglqkb.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2czzlhcyr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2bksrcaun.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2udczhxip.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ujqspgtq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2yojyhrwz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2hnngodig.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2feegmprf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2brdodbvd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2rcwfskjd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pnifwdni.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2natygxxa.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ufqyoiqb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2adtimusy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2zpyzfial.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2abiakjxh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ucfbvfnu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2lfqakuhe.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lbcyrhnk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2magyefou.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2lqotyjuy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2zidbpjqp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2itwnaxnx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zotolmoi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2qzthxbbi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mbtcmznf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2tlrlimuf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2iopyqnth.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2tqetnbwj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gabxaufj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2oszcmlln.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2mktsvcry.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2khxswxfs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2czxycrpu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2pfymjzfa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2rdebtaex.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jnwprhct.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2adhsbgcw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2gzgewpbe.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2aeagwuwx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2gyodfecc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvswxdfi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mdkypndj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2fvfkauvz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2utenbelp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zwrcquts.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2hhpwmzcv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgngpwgn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jjpfrodf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ftqvtnsf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2npurwghc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2tflriavy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2uzbskebw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ansxqefz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cruahbhg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2dyvpadjl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2pfskgbkv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2lrzapxlx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2cxmhsjkw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2mgqwlgaa.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2iuinwzwx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2vrxfpsni.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hxsxrhir.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mqxuxref.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wbmimhbn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2nrngnwkv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2dogjkuqb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2npiggyly.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2jdcxcdgz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2pheqaozf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jnjmhmfd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2itqzpnkq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2uldclsqn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2uuanyelu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2cuvhqgke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mvfwxtrp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2bbvotqav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cughuney.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ygglsybj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jhogwhtw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2hpvrrpqw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2muzodgug.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2pnappsic.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hhmlobyf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2qnbrstvi.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2knqjzpho.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2qetbvdcq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2gnnhwwgd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nffgtleo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rrgvnvyp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lchulffr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xleolisv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vivudlor.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tdibbxxe.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2kibxnarb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2phlxmovy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hrmuewfy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2oowqfaoz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ifqcidgj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2dywfabgh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2stmqzire.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zwgoipaj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2xwcmodkc.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2hagxvnrk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2tqhiysts.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2oniyhuzb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2zobhxugx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yznssmsz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hcnrpxlf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2evfiunda.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2spzmpccq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nsrqahtq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mhjzjuqu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ledbexqg.html


<!-- 参考信息 -->