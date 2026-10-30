代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgswemkl.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwujnujq.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gnibfwbal.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpotfkec.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/grfdmzket.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjttcqdku.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabrwudip.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gaugnkmth.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyiebeea.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gtotkmvpm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glzddssuu.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmjhhjmg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gqttyehtw.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkhhgxep.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/grgcgszja.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncyusegy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gfojdnnnv.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gakwqqdwr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofrwygxj.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeovbsyv.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/ghceqkmxr.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogmdutqe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/grbmlxlqv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkadiegj.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gkgtcejtl.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gonojfwzo.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gkjgllzga.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/ghplorfgd.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gfdlmqgcy.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/ghjcehhmv.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gapeitxgv.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbbdqnedj.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gipddtxpj.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/glxxyhmwt.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gokrlkgla.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gnanvbhgm.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmcddkoo.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gptwnyodt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuxbrzpq.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gntnttdyy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggbrseuwq.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtbaheik.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gpooqowfy.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gaipbsmdr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gnvaljzgp.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/giwdsrosq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gffelcmkz.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gzrcefrfc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/glfbsqxfc.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsgkucty.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtjpduym.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuofkvut.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcyraaqt.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guqzimlmc.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvayjhxd.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/grqlhyksk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyhvnsqx.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gdfhmgczh.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/ggrkivifq.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gjoxkwsro.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghzsxlex.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilimwctw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdeikmty.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gredccvru.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpjimppd.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibsnkiht.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmsoznyw.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gursceqon.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlwjeyyg.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gekkpnmxu.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnnwtzcg.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjsfxhza.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gwraabxgr.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmixmdnd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxzzhhml.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/ghqtqgekd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprskzlsf.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golzgpawn.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlxvlrit.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gnstxddqi.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnsrzcns.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gxdxfidiz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxqxosmm.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gfruvoayk.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/glohckzrw.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gcpxirswn.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gyeqhfwcp.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfygbqli.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/grbhfnfzv.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/grwiumhmy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazlcmlzj.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gzcoehzgi.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gszsdivhf.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklptlrnb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaipudso.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoemougw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gqjazkydc.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghfemgfkb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gghdcudgc.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/ggcnfmsyi.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/guwmsvtcj.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/giasyugqq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gdnoukveo.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/goeljzucm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkpesxki.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gamvwjzgl.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrecjmkk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gojzimynv.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/grladdroh.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggbyuornk.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnzzqxfd.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gpmccysao.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/geboshypa.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gjbflgrpk.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gcmdfudac.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyzuwpfy.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/guffaniqa.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/ghqgylnjx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/goywujuxz.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gxwwnekjs.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqswjxfg.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gmqstfczd.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpgplwoj.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/grydexjlu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gcqnjivep.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gdhgiwcjc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/guzxkydbv.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmqrhocf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffbrimrg.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gktyogewe.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gevowxxxl.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gywvtvhrc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gopeiodgi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/geovfgaqg.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjadyzfv.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcmzbpouc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/ggeltkdmm.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/glqhucann.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmkujhzn.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gigbnbzjz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihhlezli.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggltqqjiy.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvzyatxx.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsqligrf.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/goqnkttgn.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gbzpfwmdw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gttvoejcw.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/giejgrovg.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gcdmvltya.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gxifjdabe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gkptmqsqr.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gjseibffn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcepchxgq.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/giuxmbokj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goajjhmpt.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/givxpzdau.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghefovxog.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gwporlxyp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmqghdem.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gtozfzroz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gfdydnajz.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gksrwlvrv.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gypdbjwso.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcbjhner.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gtjsncyzi.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqfbnuwz.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gzjnfbvll.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeoqlylb.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqqujioa.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzakwdizw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gqdrwoyaj.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gwilrjman.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/grisfqxqe.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxgfgdpr.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gkozdzlev.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkhctzwa.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gbhcwofzj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlqwgaqg.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwgzrhsc.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpogpqeh.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gtgrpzcvm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoeglhuf.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjokqlhe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcirajam.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmrrelum.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrwybmyi.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbmtqhlo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gwwfzxvdy.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gjejrwaqh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gqbieobvc.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/grgvmvwlc.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsbxdjgn.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmtjuwvi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gdqzbyman.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gwebwutnt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gpsflecoc.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gappnmqph.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gkqvabfqr.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwqopmku.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/glyxwzgyp.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcxptlcq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyqkgepu.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefggnqju.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdyvavmp.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/guogdkjqi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gqrvaeuuc.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbghlfqu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiexiczs.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/guffjoobe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoazoham.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzenzsob.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzoeieaa.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwsfuckp.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaoxedsp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/grzumgtry.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxrevxxy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqyunzod.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/ghdjzhbua.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gtwetjvgw.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gocanxfow.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyxifazo.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtpeyafw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gimntnxtr.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gwihvrcrz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/ggtuqeznr.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyhiqxho.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gfsiyyuhx.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gpuihqele.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsizfugvi.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwtpkcyj.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmjfuuoz.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbhgirqs.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/grczxvosq.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gwvwwlucp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gotzkwefn.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gckfvkhbc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmqxsdmi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbzeweek.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/goklaqxta.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/getzzsmvc.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvizsmku.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grldxwckg.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuxunnmk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gcchesfdm.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuteilyb.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmpnmmqt.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkugkxlj.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gmegycayn.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gxngywylr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gffodscnw.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gpganfltx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkgjpptz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrgvaptq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gndfvoejv.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/ganrkcgmv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsohbbfby.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjkslcqw.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcpfgxbf.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxdgnyng.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggefqtjsd.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxogptnev.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/ggunamrmz.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gwakjdlro.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/geiapywab.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gcinzsvkz.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gyygcpdnt.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxghepeb.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkcsmtdv.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gybxmmzra.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqklkxra.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gauyjjesw.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeqjvlaw.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gepqxtxwg.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyndaids.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/guzchsqui.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggozoxvqq.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gmyhchoei.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkgcopsa.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxozphrxz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwptwvet.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gfohrijxr.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrpwywqc.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gogoxlnpo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gcrjgptpi.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoqswzjt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gxgsksubk.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrhpcmxi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxerojpiu.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gycwpqhcb.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/grmvayuxt.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwruuppn.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gabukuppn.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqptopvb.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/grpjlsxsb.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gatwlngpr.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gcceoasfj.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptimhbvt.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweoalwiw.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbfnagbq.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghitkswla.sHtML


<!-- 参考信息 -->