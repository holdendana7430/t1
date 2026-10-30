代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnatkbszj.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/griurchph.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gwcpfltwh.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gnldktnav.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxggspagv.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycjgolpw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpnujeqp.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteevpxyk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gurgbmfkk.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiwazqar.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwseajpp.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoayceyt.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcutxuude.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gbirzlmfh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfjwlzwk.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gmqsfbhpt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytrorgyv.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gitgsqaao.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwqdcssg.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gnmgqtpyx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlgfjhbi.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/geancwdad.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhvzmcjn.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqmfiyrvx.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkfomhrk.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gntocbojr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmlcjmhm.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gdteprmks.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/ggkpolpsk.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfvkrbbp.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbrholoo.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gknrykkxk.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsdolkxe.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrqmncsa.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhtdiftb.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekpfefjz.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/girxxhppm.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gazuzyzjt.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/goyakhzbz.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gsknuwnsv.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxfuejwa.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gltdtlgvq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gueafdeox.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gbqhwvbti.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/goxvveevq.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gdfxfhzvl.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gibykkzzo.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gkysrivqe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gscrvpweo.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvyjtkde.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gciygeolq.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmvvwucs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gcphuifuq.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkazoctz.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsffygsnh.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/giseckqqx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gcxiyqsrs.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gczwznofp.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwetqgkvs.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvlqirky.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgcmokpr.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjhcypjt.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gkkagwcnw.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/ghekjjswp.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/geoadolcp.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsddismdl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmjnbjsb.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godaucsww.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/grrynkxwu.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/ghniklrph.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gbcasxnod.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxppbkrr.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/garxdrocb.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbectsbiu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfhevrye.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gqfmredlz.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/glwuqugvt.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmtprhgo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbixuevj.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gspthsqzy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcgmwgwt.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtaruikd.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnkkhxtd.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gexzxcezo.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gaqopkdvu.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsbrolml.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gtyclbiar.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshphfcjt.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gvuhayxxq.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoatmisv.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gklybdgou.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gfosnfdha.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gpxcojxjk.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcswqidr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcintoriq.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsijncubq.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/glqaihqzt.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpwyoyrj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gacadiabn.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkaqeqmq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfplsblt.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghcryoigx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gmfrtilyh.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxzdjavd.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvpvqyps.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gerdrtfij.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbssrcvn.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkcnknlf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzrufmnwm.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlkhiumv.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnaqjpbo.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymerqqji.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbdaqgdp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzmfizqfw.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduyywbti.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbjrvdcz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkrgwwore.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgjfrala.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjmjnsso.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gbgyujbzn.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzngnlclb.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjufximsf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhfwicfq.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gypbcvych.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gejmoylgv.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkajzkpuj.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gqtbjbnnq.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gejfoexyk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/guwzmzsve.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gtlwcossl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/givhwsiii.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeehwrlo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/guguksicy.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gztfnhdut.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/giwowqfek.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmjccsmin.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuitjsur.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzywqquqm.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/goawylxpp.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunydgajh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpoprncma.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdvgaape.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getnddwml.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyxfastc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gncurogaa.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihtlmcle.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlcbhddv.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gbfgmteao.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gltitkwgn.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gimlmwyms.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlasgxcb.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gvgjlnjff.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gpjinfcqf.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gqaawsldn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpkbaick.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gpisctanh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gidbhwshi.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcezgzqs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhtqgbmv.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gxomjmvxu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gntfdjnpq.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlxlgjbt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gquwstsup.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqqeqewf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guezijftr.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgbaluyt.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gorkwelud.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdvgtpsz.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gvlyfrvcl.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnalawdtp.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/glmwudfkp.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqepyyumt.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkkmhtzi.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtlewxxhb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwshcthm.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gkatbqcdb.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gjuqwbdzq.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gnnkvlonm.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gpmdxajgt.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzzgbebw.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gejcidnfd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glrriqqjo.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktszwyli.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/givutznfq.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gnbihxkol.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gikgzjrrf.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/guqzlmsvz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzcfzcwb.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkagwtfu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoamkloa.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/grefrhyly.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/ghglspdlq.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnbjteqk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/guisdzcin.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gkhwbspuo.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gmbnbhoii.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/guwsrknxp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/geuwembsv.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnbyznta.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjzeucow.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtzjiujrj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvbfqtye.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkxmekgo.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbjidsmc.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gaplevuqn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcekbljv.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfpxwhsn.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gczcmdvuc.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/grtudgzai.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/guufiqwvk.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqmwzidg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobarpbet.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/getzcvaoc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbncdfuyt.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuswltlx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gbtftkczj.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gabbbvcye.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiktyrue.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwijtexq.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gfmvovusq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/guiydelav.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbtdlklo.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gefahezqe.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gqcrljgos.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gndbicjvq.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxflwkaa.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gecpyjnoq.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gifvdvnjb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gtpsuoihq.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gosueqlyn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflxkzgyd.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gcziubfdy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhrbgnyb.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/guokwians.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggulmkrlv.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeqkphoa.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbownrir.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufvokoch.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/grpqovecf.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gcdzgrllb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gihxkkauz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwiwzppc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/guzwhvuwa.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdsfvfnq.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gdebhrebe.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gyqqshcvn.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gxludufhg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjikoyaqv.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjbklcnj.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaizjkff.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrssowjo.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gnilunvyj.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gehnuillu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcokiqwun.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/guaipcpgk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gpkqthtux.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gewwloaca.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfprvqbs.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakzsegbm.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gbsztpuqj.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gnbdcirha.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gxjdxgvvl.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfnqnwug.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyjeolxc.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/getdveocd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqetwirkg.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gyhudhrsp.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gxxsxecxh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpbxvhjz.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/guzfmkded.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gdqzzhpex.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvceojzyu.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gklucxioc.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvqokohp.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvnzilii.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gevawdfnq.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gkaaukrxb.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzejguah.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grczlodbu.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkwoqbyu.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gofhpsizb.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goklbicdq.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gqgjzyafj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfqifnfm.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqvpajxe.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gcizmfqve.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/glfnfdwpz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gclxbrsac.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcobobcs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gfidmqfsj.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgsidija.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxsyonze.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gewmerwad.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggatwlpxc.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjyuxapw.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gebphqich.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmjuzzkw.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/grnusylyk.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgbgpquv.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxynzlwk.sHtML


<!-- 参考信息 -->