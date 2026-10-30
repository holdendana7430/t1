代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzapjanvg.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgsyqxof.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gikllenbe.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gxlojasyv.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gaqkyxcth.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gwatwsjue.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gbkpiwsjv.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoaueuhz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhkmahnf.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gemrtxiax.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gqdczedee.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcfxqebn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqfdcdvx.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyaslntq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsoxwipj.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gjliecwau.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmywzutrd.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gugmvxosl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gfcqxaris.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gzovuyhbb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gwkwhszdq.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/grchmploz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gojkxsxxt.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdjlmzey.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gvtovkdyx.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gdhzavcvp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyakekqzp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvbvpgca.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gwikvjtsk.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gybpteyvm.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkxfueyg.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gxhrefdyz.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmwrxtbp.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gdepahovq.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfunncimg.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnkssrezt.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gtjoehuem.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gcafgzzpy.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gmmuwfjyr.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gcvecyisq.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexhgutnx.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gjouawqtx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhdpplnl.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/geulldhhg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdcipktie.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxbddeqh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegdgbwlg.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gmlwygfus.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhipnilv.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/geskusyby.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsifvabt.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gvstiwpyc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gjitpmzyi.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gqabfqqjh.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvemxrsm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbpyxnob.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gmrdrmtpz.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grvrnujpp.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/giwqfamfx.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gjqexmumw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gnqiksxcv.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gkbzqhkaq.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gcvwvlele.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzabzoat.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/grfmkpfyq.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gttejlnnn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqnudokk.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/ggqhotecs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkwkwaat.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gqcxdzguv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gsergonuq.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gwoundmnq.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaccydgq.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkzysvzr.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gqocfyeyu.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gvylhhtjw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaraazrs.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gngsrzfst.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjeqjwwu.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyztxoixa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gpxivwdha.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtrjfrts.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gezqhfhfd.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gwtnrnehs.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnumrltn.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/ghmscqegs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsymtdtx.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/grxgcrfwt.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gvatkygpd.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqjcxxjz.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gidcjwglb.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlbiiqim.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjedsboix.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gwxbzvaod.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gklfenqmb.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gxfdlqaml.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gpysrqthj.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gxalstmyx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grijiiqdr.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gftzeomsn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gikbrbpta.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfppuswgw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnkjaysg.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gezlrujsi.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxpxwtwu.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gpwbywohq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyvaysof.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/guounlnmr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gpxbxfvqo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhhrbvuq.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gutrplgeg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnfomryu.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gorchkszn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdctzubxh.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gedgiickh.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gwednwojr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdsvcghy.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gewiothrp.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/guhnbattb.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/grhshjjjn.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gfohzaogu.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnhdlrhk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/glpswsqda.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwxcejvx.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/grmaqhiux.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gebcoieov.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/ghxnsusoj.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtysuswp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/guvxjxsol.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaeprnxe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeccawjx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfblibtzj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfkuagnn.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gzarqwuze.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjdvbevk.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gikpmlzfz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjekohju.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gghqlcbbi.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giafzqode.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcyxpkrbn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghafxjgif.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gugnxpwqp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcacfeyy.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqipgtyg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnhoootr.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gcxioghmj.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftdjdgze.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/glrnvuidl.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdskkkca.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvmfgzxe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqnwbngr.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/ghqvktfyw.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbewykkb.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gzzprmgre.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gjinxaxxj.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcrypkly.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaqowzmy.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gjhyjsvhj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyktijptr.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gofhxtujy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpckabjsr.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvelnciu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpnwfcon.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gzpzdekwx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdjshcfr.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggubhcghc.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/geaqdsuix.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gnszserwb.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/geatgeklf.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gopzldowb.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gxvojczhw.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/glkvbhoaf.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gobcveduk.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbilcujbr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gixidwxff.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gzivnlyst.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gimgxyfgg.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazrrtkak.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gldururif.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgcldbdt.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/glzmvlwrz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzhzywcr.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/ghgcouyvd.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeusxjkx.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzrpcsda.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gummhopuf.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/geedazvnz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnepdaawv.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdbfyhhw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwhbiemc.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gcuarrobg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gqwhptrbf.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gjuakzqgm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginhivsgk.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gbchpcbzs.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpdpmqjm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkixyvix.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzsnusid.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gsandyrkl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/giqrbsjlo.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gplylyqpb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqrapaaz.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwtachel.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdmwfiag.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gsbnbgaer.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgmfetqm.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/ganokzopd.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdrrmzhqg.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbnvdaqr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gikaelvao.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpikghms.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsldewqai.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gsibowejz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcnwtkdtc.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggxvimrku.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gytvkmqgl.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbanzqrsa.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmijxbfs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkpwhizo.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcabhkts.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsawcryq.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gshaiijfr.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjruwfeo.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gradlgitc.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtkhalkvr.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gjqejwkyx.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gmzdpfhtx.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqcmrumb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcvxuaqk.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxodkefg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gtslqybmx.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzhxotcz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmotosah.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/goqktqglm.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gynebzjfv.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeqvdpbt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtyoocgd.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gmrcxdigp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gnruqbpyq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxshvwqj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/glblrddiv.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gaajhskvp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdfqyskk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmajxfyza.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrjhxyis.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqiqxskq.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwbcldok.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gmpenklct.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcrrakzi.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/glwcxhdod.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gmafnxnuv.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/geaebthzh.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gsqsilyvf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gmvwxbzyi.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gaslttexu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gaboybgss.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gellapgcv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gmsythsqn.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbmxxuxy.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gwkusfhly.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxinoyinv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqfycyds.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/geizgkxdw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gbfqtfsvu.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gomhltenf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gwvywkbxm.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpnhsxmq.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ggqnmdgza.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunlduwia.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gskwoowim.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gmpidgzcf.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glalcizco.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gacmsvplx.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/grbxzavso.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkahobas.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggouqrrcj.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gryxnryhg.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gerrpdlxu.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtrjycpm.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/ghgdtlqfw.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzlqehev.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpdrdihb.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gkhuoeqxd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gebxpkfaw.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gwuypmmfz.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhujfqro.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdznvgag.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsqjhafa.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyndnrts.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvpbdpju.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gwngftiru.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gjdpvalvr.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzllbzezv.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvjrcdfu.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gpqhxazru.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdalibtsb.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gxlwnmitp.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/ggennyhts.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/ghzndlkte.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/grcksniug.sHtML


<!-- 参考信息 -->