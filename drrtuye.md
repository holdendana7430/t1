代发 wailian999

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrqurmqg.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcaqxmbu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gqcciosmg.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/grrmaeebp.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/ghlurcbgo.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/ggwevebgb.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gshbncmvr.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/glmvzfdof.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gteklcokr.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrpcqejc.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gomtbfsog.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcdyejtz.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/giztzznga.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gqtnsuqhs.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjvpzcbx.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqymbiwue.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiqqyhur.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gelkmiwok.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghselhecd.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdvnounj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gcxodtgsr.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzlolbki.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnukysqgl.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfevqvkcn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/ghvhhvjrw.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gbwdnhvox.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gexwzdkqi.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/glurxsqnh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gqzypjpwq.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/ghvqpqgsn.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ginohhmia.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhtodfez.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gapxyxchn.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzxkkqpvs.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gogwsonyt.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvwiwddz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gqhsrzfpw.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gbzkrkexc.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfdjkiej.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgmezeqs.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxznvlyj.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdvwndxv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsvzhgij.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gyccnhcmh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gobbzkgpd.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/geivwvbjv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslehlfhr.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/ggwxgfdbq.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gapsvahur.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvzqclxll.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwredsjt.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqenyuga.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcqmfski.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gmquhuisi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gwknvxyor.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaymnkgc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktpgtbuk.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfnyucmv.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxjpcwmr.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvvsyqgk.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/grdenotey.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbwqwvuv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkemjjcu.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gmpzkrqek.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfpsfzmx.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdihotvby.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/grqfhwwfh.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gwokcvoqo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnjvtlie.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gciwfnrgd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/goyjgflfi.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gcrnimwrm.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gpneotpib.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gjikqtokj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gocghpbgh.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggxccotnw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxhiaosw.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grgofnqxv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gbsqgliaf.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gppzlrqnq.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdosnhpe.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/glbiqpwgs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gczpmmuyf.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/griougxpm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnxfxqnih.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiqbdlvn.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvqrymfy.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxkbhzfd.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/glyfbcmgd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/goncuthga.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyqsypdu.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gaytorzhu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuouolyb.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gsomuhsll.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawreilqd.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gthhwtyfo.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxessneaz.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifpleima.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gbcsyjvld.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryshbuvz.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyblqxfq.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gxautyjcb.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyflostkx.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoanlxbp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gjhasjsxz.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gisbiwrpq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gzprpbyps.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbaiggca.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlvtnftk.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuupctuv.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxghezrlj.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvivvcwtu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznsjiwoy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gveqtdjon.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gklkoormu.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxoksbtnl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gcpsugdfi.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/ghdenjefw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/goelfroef.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/glgnugjye.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gvlcvtrfc.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdkmruvj.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gtlufjnjz.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gyizdtyja.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/glnjcltig.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gqkfdofor.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gpwbebnjf.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gwyuvowzd.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gssvksrlr.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gnqeqjlfx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/glgxtxjtd.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gycktuzid.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsraplrun.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gkmdhugqj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gkqphxvrm.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbetlsptn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gswecltxz.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpqswigo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gmbvkwauu.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gdnmhkxtq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gilfuoyve.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmhuwrfq.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gblxysfdy.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbzakryu.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/ggnzoctzu.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gujfseeyy.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiigyyji.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghntzzjrj.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gcognvtwh.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/ggauaevub.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyozmyuys.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gstjeyixt.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gdnmgswkj.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkfsqhnk.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gskxjebub.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmukqsbo.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/geduxpbdm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gejhpgdms.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/goaiepqyx.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbgirkgt.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/ggzdhnxss.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/goguqlswa.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqhwajww.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gleulnray.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcsurqoq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gsgvjxfbl.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdutmbgt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gbvvwwfya.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnmohjyf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjtormkx.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gsaupjmfv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbwsbjau.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfgyrecsl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gnukkledf.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gvdcxznel.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkdbbbak.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqvjdofvk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gsmckcyek.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gecrpccqr.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/ghpibmnil.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtrjlvbq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofxpqsmp.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gwoqykdkh.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwhlxawd.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcskwuvv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/grlmfxhmt.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gimkkfshe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gurygpoxf.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gnuwoojyt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqyuwfbzt.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gykzoaryj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzghkqvq.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojwvemvu.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gibbpzmtw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gccpgzafs.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gporqbwyu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmxcybrl.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gizcpeaem.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gihpsknjq.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gnleemzhf.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnpslkit.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gcwdpqfjm.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gddxseorm.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/grcngodbl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvdbqwao.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gkvprnsuv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiullngx.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpymqyqb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcyfmemu.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyubqqof.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuiceabi.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgsyczzq.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbvyaeyv.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gjafzyeoo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gixzxcurs.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkzdbfln.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gvufrgonl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzrxgcwy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/goalyxxhu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gamtwvwpv.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gynyebkfw.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtamysqp.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gburhexnr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdixumhrh.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gqlosobru.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghepmkqmd.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyngiftvm.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gobauzxjn.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gxfhjatbe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/goykuljli.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuoznlmr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/guuudmltp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpmughzk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvweffwty.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbshgtqx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwuxqicn.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzxrbrmcu.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkptucstq.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtramvym.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcybmkwhf.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvauauppp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfpfuzga.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghguuraba.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysldixop.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgkovhur.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gsrnymsjl.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlxgqfub.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdtrwmxd.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtprxotxu.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gliqgfctt.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzuegzdx.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsakbnkco.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoqcpgwd.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/guicpdjxv.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwgylyzi.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/goxizemcz.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gwcebrxth.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmopraul.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/grfcyfvfx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjcvlsso.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gryftkmzf.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gqjvdbiyk.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/geifpcknt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejwgkuuk.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gkpkmsvpu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gebbjdtpd.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gueorrtmc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlucjxys.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxbqgavu.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gykbwenpu.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gmadeqdbs.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gmyffybec.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gzkfbsduq.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrcyfcao.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhzrwqar.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkwznpka.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/giygpbzyg.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbxywxps.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkxjwguv.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkjapwpa.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gunqnmeyy.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbkulszg.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gilnotgvm.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigaehsno.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/guforzgfv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnomqblw.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gqzgvlusi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gkpquvhmh.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gebzwleze.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gerkdgynb.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlhjtpag.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxsezwja.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gmhxngdij.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxcdnaqn.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gamhmycfu.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/ghttsqywa.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gipswzmbz.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxvozqov.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeihmcbo.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnfiuttx.sHtML


<!-- 参考信息 -->