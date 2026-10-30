代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzccnwrd.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcrmcrss.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbugadsv.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gerxgatyz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gvgvdlafs.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gimylwrvd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gctijpsjt.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gorfiagbv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gvvwjlxkf.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaxcrrfq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gpdzgyefm.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfccddrw.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmacathjn.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsvpbpnc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/givdwdihr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlejjagz.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/giyvuexho.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkpbzjji.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gyhnkddyg.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/genwvaosl.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvrlqpey.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/guzonakuw.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxlqinkw.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgsoowna.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/glzqozufh.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gieivljzf.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gqqdownwq.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/grujybicl.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqqudkwh.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkgimbee.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gwebftiqn.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/ghdbkyxsq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gkjdvafim.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/ghzbshopy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrkkmexu.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteynyrkw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljteulre.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gotodhscl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdglgpcj.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/glmkhlffa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeurqltw.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoqsocwj.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ginkkwbjg.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gajawysbx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpulzinz.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbsyltwt.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmznqbui.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gzaskkomu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gxrusbpeo.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucmawblr.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfjqoihw.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/grhtwyxld.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gezervhns.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnelztbka.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwijvbyco.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/ghhbwtzih.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gpasvqaau.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gmneestph.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gadxcuuxn.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoolwuij.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/girmmpppc.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbmrbdkci.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/grmhxpyuo.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gueayepns.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gylerkdpv.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gldudpvqe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkmngbut.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/glvrkyhze.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxbnptwv.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gergrcvle.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjgleoip.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gxroizpxs.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhqbexrj.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnukwwyel.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggeturfpz.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gudpauvyx.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gbgscemet.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gygqukbsc.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gaekfetvs.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshojpfke.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gurvimjow.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/geqqvlrob.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxipylgne.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gtganirfp.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gttdcxyyr.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpbyjcoc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gudvsvgfj.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gicnhjjhn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugjyxzwj.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuibpnuz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/ggvhnbnck.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrlmipix.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdejubgrj.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gvqphgdta.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdgynpmj.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gxjeffilw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gstjlprdf.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gawmcfznc.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giawkddds.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdzekpzue.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbyljsfv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvxipnxd.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gyainvheo.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqwwpror.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjypnmwuv.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwmvonyf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gketxvkkv.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmsrtvbh.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyjtbtxh.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/guuffntzs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gpweeayvk.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/geytewqam.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gbeubqbco.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaklggtm.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/ginylxblu.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebptnyri.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmtzwhqh.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gyxgkorbk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdyzwpef.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gfijsxynr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gqqxjdsfx.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gphedylig.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gpbjkfgmi.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/guhnsoqso.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/ggktcgqzf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjbirvuq.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gdzalrzxd.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfbleiioc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtikqdgcr.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/ghqjcpuke.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gfdjbagrg.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/goqtleafw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gyeunabjs.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gslajqqzk.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpycsbod.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvecqvjf.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbswfkgck.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gnezilrey.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwovyjyp.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gluvuywou.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gssqeifjy.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgzkazol.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gdcwbezqx.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gstgtiysu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gcxtiqhuz.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmocbwcg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/grcfuicxs.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjpnwipi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/grzqutwhk.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnynduqai.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdajhsxau.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gxdofepmw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcfsktnn.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gjpadaxhc.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gwvtxiayl.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gaatfflxu.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/ghwwkbywt.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gyjabxuiv.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gfvezgtmx.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvapvbni.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaymdzxqv.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwloerovt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gezultwnk.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gwdngyimd.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gzadimitq.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeuorueu.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxhmnhou.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gfbaccelt.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gcffuyvcz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbzggqew.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gjedbcnjf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxyixjbt.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjxyylxt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdudqfrbe.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgjevjme.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkslncfj.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/glwdafizn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gjmxdsxbw.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabussnrc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gtmaxbkyw.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteiatjai.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvuvrcid.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gpybxapaa.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gutitlvxg.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gghvcrzbo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gbiomjity.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifhphvyf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gvnejskjv.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gowffrcrs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhmxrpry.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxkymxrdw.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbilkika.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gqmvngfjw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswxsjxwo.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmllpxbo.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gccwkuxyh.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gmjlwytwv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/grscuymbq.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gavrcidag.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdllfzgbv.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gbmxagpzc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glegnlzml.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjisgejdx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjegehztz.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzjmpwid.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhoexixh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gspqcpkoe.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gntrkznsn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gbgltwlrn.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/grtfzoztb.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhercsmj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcorlzmdz.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxnjcnhv.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrdhygyb.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gafjifuah.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/geaiaepla.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyieityr.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gexmdjiub.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgzqtxym.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gbzuuxkdn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzablthv.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzglzmrx.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gnfnrrzyu.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtjmpnwy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwujqbub.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gckvqximt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzlppiki.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/ghgujbqqf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/grmvqiqnp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gaowynqnn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/grgiiemix.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggsfivzpp.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwobvwpz.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/geltaewdn.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvddzpryp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmdcmppm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucalwgoj.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgnjqelq.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gjzwexkii.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlynutxv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisdkoztz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemuzqlph.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesoslktg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/glxuxoweb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsabqrwdz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplgsuggv.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/giesnjztx.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gahfhlpkh.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyfzvznn.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnajvosla.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbxbanpy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gjeainuaz.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdhsjyrr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gizzsadmx.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gkkkvxlpr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqahnruo.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gfacfdmau.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhozbxqu.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdivdenzd.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsezfcir.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/guimnxyaq.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gpyrdmoyt.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gfcxiikxz.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gqoprwabp.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfpfnalf.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/glwmvsbsh.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsnycakm.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrmdcmcg.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/grhffkoex.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblizcrep.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gcclivodf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwyhcjhp.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gddqiyuwh.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmojrktmq.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnqpnaos.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gmwrmjklk.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gttqgzsiu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gteuolegk.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfutgtci.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gckzwtgzk.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gklbzanvh.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gspoyrpyu.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuhbnbbl.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/goereyqso.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gmntjdwdj.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/geyqnplgm.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gijghkzkf.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gknjyriho.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpsjfxri.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/ghjoaamfm.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjarvhugf.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/ghtqtujjv.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/guvfudtug.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gwugslibn.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdpdcadjd.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gzfekksjk.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnngjpoh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxoniirs.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/ghgqdmxsa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gldmiuffh.sHtML


<!-- 参考信息 -->