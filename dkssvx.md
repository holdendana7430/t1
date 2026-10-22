代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ynruycuh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2mljybzfi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dlttatun.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2hwchfiub.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2jbbtxtqd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2phiwjixz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2opwrbjvx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2eeblnwil.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rsjqufur.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2garwdxsi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2rmeupnqy.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bcimwdjk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ldphzred.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hbybliil.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2rbbdcmga.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tmzjugpm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2mumzquyz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hlqxtffs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2nvwcxvlq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2stqrzbqq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2qwgkcgbq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2cyqubmqd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2xelxhgxl.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2qmetrnhv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2fkdtcpxe.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2anjjhbzt.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2aetvjedn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dktldnqe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ucutomov.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nvbguxfq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2afkdbkxe.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2lttbqaki.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jljbbrxl.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2skllcijw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2izgtrhuz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2idlhniyt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2avwqzmct.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2qgxudtne.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xlslycuv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2klnfeunx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2tvocogbh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2zmdehccp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2pgwkhetk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2kjofxncr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2rjwtmqyz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2sxiwfemr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2bwaqhbru.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2vuylqbou.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tepvbjwi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2yrlusrjj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2yngreoze.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2kwboteyj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gknnldwe.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2laddtlcu.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vebbtuuw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2hzjvfuwo.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wifhxjkp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2zhxrcrul.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lfbxphku.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2qxyfxylc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2gwhixyyi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ximfsihd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2kxwjhowz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2sfuwczhd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fpgwmusk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2isbhqtom.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fecgnfvl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2rztbzeup.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2gixyvzgh.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2lmuifhnc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nahqeznp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2yokiidap.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2edxmfqis.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2dpvqfhxj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2thdumwzf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2nlwwudpm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ftuktuuy.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ypqbclxs.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ifcomwzc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2tqipmlvi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2qpryflop.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ycxzqpeh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2vzczwofm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ggatrqrs.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2yozvtjjq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2nvmpwnpk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2wkqawzhp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ogqsdwsq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2bdilljll.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rfhlthrw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2daolecwu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2zdxpafvt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xqvgnydg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2mhbwxizt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2pozzuzie.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2tdbxboyv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2adbjiedx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2owjntsii.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2vznwnivh.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2tvxajiqx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2lkbsyojh.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2zdrbqsdw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ixbamcfr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2iloymcwv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2sregjnou.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2xfvttrhz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2slqlpesh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2buvtbbyi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2yvhbqhud.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2mxmactra.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2erppvhky.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fqdyycbb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2cqhcshpr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2bbcefjuj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yypgedya.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ukukdffe.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2spupbzdt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ftixhmyd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2txyhanwu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ekcmrgzp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2sqwswrvg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2jphyvkhj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zkdsazmi.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2hfrriqvk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2jfykunww.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2tdxhmqsb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2mjaxnmwj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2bkggkxqn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2tgpthncx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2rjrujplh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2afsmailk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjnucsup.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2idcjyncd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqtwgkel.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mjgbyimf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2bdoosoyt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2inlrggmy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hejqkpzs.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2roqscsrk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2enrduape.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2xfumrjat.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2rqgppcte.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hzjyesgl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kryzxqls.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2eopcnxaq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vskdsxah.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2fkmwowzs.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2pdlqjwbj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2oyhmezzp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2loxwjuor.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2evqqsmnk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2qwiwzrjb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2gxdqdzyw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ltpmgyen.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2cvczwood.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gvttqsaq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2mfqlglsz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jhxoisug.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2noboghyh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vwtimzdi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2uiwujvak.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2jufjvvao.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2zuiscsqo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2xuqdvzcr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2wgzkoeuz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ghqktbjv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2eyfwgeae.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2vuydufks.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2chbabjzm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2prlfvhrw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2bpolctuk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mkekjlca.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wdboasdc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2amgwiolo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lgrbthvr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2yolcdjul.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2edmdenml.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2jugdyjlq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ksntdwvt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lijsurnb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2bxggzuux.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2zvrzgfgc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2smujbtxc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ewhagjhl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2dnbksazk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jtnlkcag.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vekocbtq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2cedcoagt.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2rqrygnxu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2stmrqbde.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gvdykzvn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2zhvdkimf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qfstvyjo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2awmfxgox.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ytyofxho.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2solvtzjg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ndkapfuo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2aeuaqzru.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2tmaxmrxt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sujcwkml.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2zessxisf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdwxzxls.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2rotzcucv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2rbwulajy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2raybqdai.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mtwkiugf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2wktsdhzb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rubmbnaw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2foqrzxqp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tyzsfcxs.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2zxnoiytn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qzxbhmpt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2jkgbtzaf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2epsvxhlv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2qbqxdixd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2canqwomk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2nyhjjieq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2bxvtyugp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2tspmqnqq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2yvxqxtvw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ffclbzlu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kikmkzsp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2cktnmljr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2agykopst.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2omnwxbcl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2wmggczfq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2jingpzsw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2vujolgyp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2lkbugoev.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2obnxyjwk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2pdfhmbuu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2qxrxkrki.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nfdhtuhh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ahfpnixf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jdhrgyck.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2nmqjxowe.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2rpbhcmio.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2etmqefat.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2qwhqkeih.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ewhntrxb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bujqvwln.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2suyycxue.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2pehffdja.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2bianqqno.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2cpnlkczn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2oahkinca.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2pceeymzt.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2zflfxdah.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2fxhxyfia.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ublqpcax.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zgdbjtxn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ivyqfdbe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvaexidn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2rpyyigse.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2xldovtiy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2xqtaihuh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rvzkcwcp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2vxaqojwz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ylojywav.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ftgdugji.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mmqemddg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trtmwxsl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2hgyklpvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eyluspgu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iijblxjf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wzdwipod.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fuebxzua.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2eosapruz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2rgtwwwys.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xmlxnaqi.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2lnfcvtrv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2iuzhjjdd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zlojburb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2enoiputs.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ehhccynu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jarqjjex.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2eyshribm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2csnsqppd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2dmarnkjy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rsnxdwwf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ewxaunpb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2zgqymlgf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2jhoaszsb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2uvhllufm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2zjxtdokk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ibkjfvom.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2udovooto.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2itgiujal.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2glsqpmjq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uoazmqep.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2tdwtdnde.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cgdfpmdc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2chgrmgkp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nsqdscom.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vwvrdpjz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2udpvraic.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2xagtngot.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ollhgfzs.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zarkcyzz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ixsbwmqo.html


<!-- 参考信息 -->