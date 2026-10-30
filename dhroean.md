代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gmhnvrlnr.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gtrdzfkmw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/ggbxhpxze.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gizpocjsg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/ggzcwaalp.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gyynbollq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gumfojnqo.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gcyfljlhr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gtqwaifto.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gugrvzjce.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gjrtzwpoz.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gtpwgjklu.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gioiwzzxr.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gffwrfhul.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gwehujmos.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gyslafqqu.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gfixgesgj.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gbuvumjoa.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/geydbszhb.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gzvliwflo.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gdftlgjci.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gcehkilae.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gmigmcddg.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/guvjikllm.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gfbmroxyl.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/ghffgxjet.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/grithttgo.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gnyfituwt.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gxbldupie.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/ghnbekztl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gpfyfaxsn.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gdcdoniyx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gnscwphee.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gapoegfje.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gxyikyhfr.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gnjhlmmkg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gxudaiwzk.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gclpkahai.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gtjtkochz.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gkprrdnza.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gdwypldey.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gvwspynvt.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gbczhghsk.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gzuzqywxj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gwfyohiur.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gszgsurys.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gniucemqy.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gaaarevck.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gbvbqlyot.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gbxnhbblv.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gwfahyjjb.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gzommcxgy.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/guesrofwd.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdiineyio.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gabcqboft.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gnndulzyt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gbhmfwkoe.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gtrcbdulv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gskldgczz.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/ghfmmblpr.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gkmwlihmv.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/ghglgurno.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gdkloaasa.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gmwjmvdtr.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gehocsieq.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gqzggrjlr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gkscgqhmx.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gvbibrrmh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gdwsagqjn.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gbwvnbldb.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gmxkqgeup.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/givqxswqp.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gbvnfipap.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/glbpdobnl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gqthfrcdb.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/ghoqtnuxn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gxpegillw.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gckkyehbq.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gvewrbxvl.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gtfonvmdv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gahlhmdyq.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gqjtkgxkg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gghghlnrv.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/ghljjkmvz.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gpcsqiyvr.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gcttrtwjb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gyrakvkrg.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gupjcantf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/geecwwmoz.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gbynyybmd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gwiqemrla.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gokldjdud.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/grxlqbwkt.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gqrcynfqs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gprolliqu.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gqmtyopsd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gdcbadrzw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/ggjxnrtev.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gkmpppgtr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtditgbdv.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gpzcbzdtj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmpmerukk.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/goildhmrh.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gofrvxwch.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gjuymjyzy.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gxqqswfia.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/grvxacswn.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gabeegbuj.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gbqkokoha.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gimmgnoos.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gljgjbrnd.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gajetscaa.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gxjtahhnl.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gqfoyyiyj.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gwbdbarfe.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gtwyhsdjp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gkzdbvksi.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gdjlorser.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gxqgastiq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gqhsyrrpp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/giarnwedl.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gmgsbhmuy.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gwpqclyjv.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gcrldgcux.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gpmkwmtpy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gzvdeqbol.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gbpmirwrr.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gnfgmavbp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gnekakryn.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/glnuxuhcw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gihpnpbti.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gayzwkprs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gocnkewel.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/geykywyar.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gxutwzgio.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gfnubbfjt.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gpaxkifts.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gcthlgywh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gbvgxhiea.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gthkvaajy.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gjmkezcop.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gkzvzidpi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/ggutqsbnt.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gjqclcusi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gcmeuekff.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gkairynwj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gcnhptxmt.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gsbtksrhb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gsphpbmth.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gxflkaksx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gpqzivdfx.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gieiidcyz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gqbhhtsxq.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gclphekod.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gdnzakyzl.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/glkztakvo.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gdrdxbanc.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gntsayxpn.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/ghhintdmm.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/glxytbvpu.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gaiawwdyg.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gkptcpwcw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gtegrbadj.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/geritksaj.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/ggweirgev.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gkyvpvzns.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gfvmpwecy.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gdmeyiolv.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gebesgyly.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gnqpipwka.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gvhlvvofa.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gaefexhyz.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gzchfpwau.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gxftvjnmt.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/grnufvsou.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/ghlheqztn.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gbmgkuaxr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gvsetfftb.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gfngypzdn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gnkhqthgf.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/ghofkefoq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/ghtejrpjn.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gnxdleljt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gnzzdaryu.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gbjtjpccv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gwjfgsesv.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gfzghzqyy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gpkkncqbd.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/ghtgequsy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gqbnsysfs.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gqxrnznfq.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/ggjzcjpzb.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gsuaizvpu.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gwababnza.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gfyhgrewu.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gsfumimta.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gppxzlchy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gmwvozzyn.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/glbpcpvol.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gyubhhzqb.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gqxshbhzu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/geafyxqqk.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gkqmghgin.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/ghsydtiup.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gsytlqmft.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gdnzyqgch.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gmvkjamoy.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/ghsmhqffv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gtkbcbywc.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gfmoshvrq.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gyzeqowyr.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gfykmpxzg.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gussyxhpy.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/ggfxmwivk.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gvinvfqwz.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gnfironsb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gpbcqotpc.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gijrzpmja.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/ghmibveft.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gcrfonkbz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gczjwlhoo.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gyxxhwpgl.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gimkmfiei.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gxwkobpip.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/grynkzrtq.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gesmmeogj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gvbfoizrn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gposaicsk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gqfqrgdvs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guhgppkff.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gzphyxeqc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghqlrytvl.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gtsjldhow.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gwcdtdrcv.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gkrlumlgp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gzjiobeoe.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gdzokfjwv.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gkzbuflwh.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gsljlbtyx.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gacxpymsg.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/ghenurksn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gkxnragft.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/guaozmmqa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/givtacdtl.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/ghaafbyip.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gbczzmmmn.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gdehdfsan.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gxzodjfcv.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gqchdtbke.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gszhwzcok.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/grsqllfwg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gqzpskmyi.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gqlnvhxaw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gkohsxzur.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gxmeudpyg.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gciipbudj.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gmaifkeav.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gdlozjguz.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gvwapfijb.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gtcfcnzuq.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gdupdzkpa.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/goytwelxe.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gxieprppq.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gdxyircbc.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gobityrvp.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gdgukokov.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gooaxxvah.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gstrxsbbw.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gvskkqiwx.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gvxkjldtw.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gzlkvdwom.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/ggnvgdjaw.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gmhuyrtrx.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gerzlnmkb.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gunyjiryn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/giimoeyzz.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gvlalfbwg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gyicuwdcd.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gxvbkzved.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/ggalcyxqc.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/ggnqgoxig.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gsrzeydkr.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gieobxtth.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gorbsrxtl.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gdefyxkzo.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gkcdliveu.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/glprgozfh.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gtarqvmmt.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gptqciwqq.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gptnpsrag.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gagemrdre.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gqxhnclad.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gtdskgvgp.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gvqaltmph.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gbunlvynu.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gqvvdfdnw.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/giwnevwhq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gwjymhqmm.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gfolnbekf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/grhfkfimt.sHtML


<!-- 参考信息 -->