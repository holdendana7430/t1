代发 wailian999

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gerkyhjlj.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gxirupavu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjirlifdv.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaycidxh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gijroypzv.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gzswvvlfm.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzywaloz.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/grarieflo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gzvtdspqk.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gyoaabqws.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcphcvdzb.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gwirywhqz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gjefpepae.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwojhrdps.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gpxyejuug.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntsecsgx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gftcrflhq.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gognuihik.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgxbyorf.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gvfdwjwfq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/ggptbwpos.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxxftrlb.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgqmunzu.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gptrszjng.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gmgvyorbx.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfgmtwpn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvsrfgyj.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gpiyjcmho.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gcgmcjmea.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gldgreyor.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gflmayedh.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gessxfadr.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/grltdwuiq.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghvvxycnu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnxvtzhk.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjihcgobc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkoosovi.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/goezyyoyv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/ggpidsykn.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/govuymdsn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gfmqpmxre.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhbfbeez.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gwujehizf.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjzlyixz.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmfvaidh.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gswtiljld.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/geurcffbi.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmflwfzy.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gkyrtzyrs.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gqctyfxpm.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gcmramncy.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/ggyvoubbq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqrexvyo.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gocyjpnlu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbhhmfnm.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtmpmnyj.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gsofsatbc.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gifdmjnpr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxjnyxcy.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnrtjfpvd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyhzxjrp.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwapwtuym.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsselrld.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gfgydgggl.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gyvocicdh.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/goxkdhhur.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gxnmvgqqg.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeuncuxf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gdisrupmh.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gjojycwks.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gqkpwfsba.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjmbzyvk.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/ggqlgfvbt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gulbytbho.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnvpjqpf.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfexkhjgm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxdgqgnr.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/giouqenbv.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmkxfxpi.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowfrjdtv.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvxgytox.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvwxdouo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaumiwhc.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gncurmshp.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gkjrnnyci.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gvhozdkou.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulbpxkwe.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gsknginfo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/grmzbjxcu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqvikyxa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfenqdxj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gkryhhtnx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gjnkhkwvl.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/goyeqbkhf.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnrfzfat.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/giolwrrxh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gvyeppmup.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtvzlneu.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlyiyclx.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gygpqejwq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwgeblkx.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxbauhyr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjjwemxn.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqsjkvve.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjipkvhj.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gvtgquzui.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnylxdob.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gyynfilkm.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gjodcvymr.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gjykvlafq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gyxevjgfa.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvfuqjjg.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gnwmkcych.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gcyzztnam.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gpvwpdwgk.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gfalmtpsi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gggcuvylh.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxkoywzk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gmfuvfghd.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcgbrncq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwylrqlyx.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gaaoinejw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvbumztt.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gggcqggwu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/glykvpjwt.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gtyrtyuhb.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkjddaqc.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gncmbswlg.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gpondtjpz.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gespcuhlb.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gfzutmhxg.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqdlfcrb.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/glhbrzxzp.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvkjttmhh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gzxvvwuig.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpihkivq.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/geqsvbihd.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gklxqrtnv.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gllpbyigg.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmqduxnl.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcecmnmy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhjnobkq.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxxpjhso.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gersncxta.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctuqxogd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gzomqezyf.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyvruwie.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbxacnrwx.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdaqmzkk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsiazlnw.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gbobxlqwt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gozynxzju.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gxdezlpmm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdskfhyhv.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuxjipwe.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/grfowybap.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gepmcdkro.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaijjnzh.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gvvgrgjwf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gzfmdhfrz.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjchavwfg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/grchcwdcp.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcteifnc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvaxwmzn.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/ginjircqi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/geyjdjtuk.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/ggycmdtcd.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/geqidlgss.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gosntmfzn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gqdlblcvy.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwvexnfr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcjezxfl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhhnjrue.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpvexaoaz.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtssbikvh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpglndipy.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/geeikfrqr.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gddaqkjnr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzfbbwmq.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gvwzlkgid.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxefuladf.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gzongtejd.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gkrrbxpmd.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gvwmhhxuz.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfhxztxrs.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gfodlyero.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gopnrkrzj.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/goufsiqnk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gpeydthyf.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzqytnie.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gbcsaanvp.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gwkptkbay.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzoaudoqk.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyorwlic.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gnaghgkfl.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgcblgbq.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gxoplctnu.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/garywpfza.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gbffxgbfq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjemixzqg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gresybihv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqyzqpmv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxskypgn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqoyyiiuu.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/grqzgcvev.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxwpcxgd.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gymqifogo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gqtlsviqr.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gkunhcjis.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gxbglvnaf.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwuaylul.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/guhbtnteh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdowjcxqw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcdqartw.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gvarklnls.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gstzfmlau.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/grglwqanf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gebcfxnmj.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gjzyjyttv.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gfxccnfmt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtmgzpxq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfrmrmio.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gaqupfdkj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/guwynfrxy.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gwunullqx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrszvwfm.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcpzrqkp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgerdcxr.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmsrucem.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gmksujxyx.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gaquxembm.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gpymgzoes.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gbxalwonv.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnmdjpje.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gqdjjpvsv.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gykcmlvus.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gjdqxbnoz.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gplqydkrk.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gvkicymjw.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gxufnspux.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/geifmomqs.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gtrswbkvt.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvtqewxu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gcxicohhs.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiyersdr.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmeabfpt.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gselpxnzc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuiwaxrq.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpanpuiud.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpidgynzt.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gjyrhuuvv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gppgadymf.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gcktztvnz.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgffbayr.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gumptdvyt.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfserrir.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunprcuwg.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdyckurj.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gjgqqkswr.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gehbsllvq.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/garrkfdza.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gykmbdfmj.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/geayxdxti.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gythyayak.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gywxwevzb.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcznimtyz.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gzunvurbx.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gxwhdttct.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gxqooxuiq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gbnwixaua.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gfpixtxss.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gugbvnumr.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtuagbpb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyxvwpmr.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqarbnbht.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/geooedsop.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gwrlopoqw.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvqpyhey.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gfdhtaddi.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhmhjpsu.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gjnoswcbu.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfphzfcb.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrudiapa.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmotfeyr.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gslkfhhqu.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnbgsbfc.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gikcoiwqx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwhhkurs.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gwkybhfbl.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gfvcwwfyw.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gmuasrlyh.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqatcwcr.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/grqwfzull.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzydsbfsh.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/gxsnzpdii.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqrtjlhl.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gcagatjej.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gadvtfquq.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gtpwwdrkw.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazfqfinx.sHtML


<!-- 参考信息 -->