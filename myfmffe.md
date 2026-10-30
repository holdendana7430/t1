代发 wailian999

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gbqnrlwrs.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfuvgymi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gzdluiadn.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfuqcxsi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gvpkgcils.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfdpakix.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxozfxqws.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gmavmeqgs.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/groleupck.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/guepytjxt.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkcmiiun.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gajhdekfl.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gwzrbuahy.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/giunsvecz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvliscqi.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrkbbvvw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/grykmkvxz.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbusuqat.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gmzjkiexl.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gqlbldyio.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gpwnpoask.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqvxyvqa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ghsagergi.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gnwwhibdd.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gufzuphbb.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqoqzzxo.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyyxxddg.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqcfvwkk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gqjixpbjx.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gyuntrrqb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdaajsxq.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhnfeejl.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiefgqry.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/giecnvtwu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmaepqng.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvxhpotrx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gvmmfxbih.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gierewhxk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gsksqetwh.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gonlzlcgr.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxwruzht.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/graqdbqtb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhxvuerp.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gccstases.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggrrfacmq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvwmlafe.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gapifnlel.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guanrrgkf.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/glripovfa.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/golkviwgj.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwlammqi.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gfsaunasb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzngqzijf.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gkossioun.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjgkhzro.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaqzbhiy.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/grwizdufh.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqtpoodc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gquaokvkh.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqldywibk.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnhktyjm.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwkxnofm.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgswzioz.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gayiewwts.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gzbhpishr.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gbjqbzvbe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbphfrbed.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueuhauhw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvymygoc.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjiaxogw.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdlbirnt.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjfjakswh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkxvycwr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gfvfynwfu.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjgqrezg.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwukqjick.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaozfxcr.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gmprxnntg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gwodylodg.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylwjdwis.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gerbrghkf.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gsscscren.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gioanpdde.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gztfqzhda.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gwfzprrrl.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/giyrlohzg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gjmxlfamf.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gbzrxsboc.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gxrgwiyme.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gbtbpcuvb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkjwgogf.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gladmxxhd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gjbfmdgre.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcghzuijv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gakwoczup.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gansaubyy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyekaymc.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfylfnota.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gfmnccrdr.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gdghpisci.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gpyasoatq.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gijxrgqrd.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gettregna.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gqakctbqo.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/glzclohkc.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/guemxocqz.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlpfatae.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakwavzsr.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/glsnjqjjd.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtagbfzvt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgjqvzhc.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gorodxzuv.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdheuycy.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoyaovvl.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gokxhuafz.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gielxntga.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gpdlfcyod.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnuuotaf.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/grqujiiei.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcniucfz.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gudyqnska.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwwzmyql.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gpxveazyc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrtqhgud.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gsozsbram.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvupnmykx.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gxjfvowhl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkndpzcqt.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gdvufjhzm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfnbxpwr.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctwerhgk.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gmarjiuzm.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gijvsaigt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaamtagc.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnqrfvne.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gpmcosbtm.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmscnvzip.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpcgjuzc.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzulpzfnp.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gcjqwebmj.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvncltqa.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdlhqhmf.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoedjyhc.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfvwgtqyg.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/goryxitxd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gelwtqfjw.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gqbukrppq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzyqxqbg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsdwecyc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gscziqyhz.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqdvbagj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gvkkhodpa.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gqpggqwkp.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpmqykgm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gimjygpke.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmgxarvk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbldgbrgc.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gqwjixjmh.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/glypmyzkn.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsccsywc.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwtdguavn.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldfeexnk.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gmaphkynl.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruuehgom.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/grougsxxn.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/grepzfmen.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gawhynorx.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gcssbdumo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcasqcogu.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfhsfafo.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzoduyfq.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gknhwjtxf.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdsprnxc.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/genkecsfr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnebodrzc.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gkxlyfogl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gblqttaaf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxreqpjlf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqgfifrp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glolgpitc.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfzvnjmfj.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnjyajtm.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grttfjtkn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsrcwxna.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhgbnmwn.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gcivbjskp.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/glyjqbsge.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghymntxer.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/guiceiqrm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnshmnml.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeeyfokq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnemqjmvl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuglasaf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gopmutfiw.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gddlnoaan.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gpitnjpdf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/grbdxqdic.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjmgzzhn.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxziuijj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/giivpfswu.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goahcyqxx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjydkqtx.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrhirtqs.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gcmtvjmrv.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/ghpndinds.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gqwojohwq.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gmsdzmkoi.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbalhcmt.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxnhhioj.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gbbszfhox.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfahjhgwv.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweszksxs.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gukfxhiol.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzmbxacl.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gntutyxqv.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgkiengu.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gasxwnxbk.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gdkzepqxp.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfagdyqc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtakoteqe.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gjsgarzlk.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/ggajqblxy.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzcrusjl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gbqhcvopp.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gphbzhxjr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgvzmocn.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjjezstr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdzdkorv.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gjrcyxrcz.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gxwgrhkvp.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxrfbcky.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gatvsanbm.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gqypqclxk.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/geqazihfd.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/glczcixxz.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gajncxwqh.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gkjwyszmj.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuccifcd.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtfyhfcc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgyvoazf.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gucglhwwg.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gryqqyjqz.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gycrbzykb.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gyinsjdxe.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmevjfzm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsvjvezw.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagnbhrpk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzspdhje.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gkaxoxkyw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gryygwpek.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/glgkmzhrn.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gmouudxva.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzellbxkz.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdydxyhk.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtcuympf.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowogreye.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gvxzpznun.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/ggilxnssz.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamcwvaoc.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gbncwnsmv.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gkxxgtwit.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gyjbtcuty.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gusbopdti.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gzjblgxxv.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/grecfpycz.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gaqkyxpan.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuehqodo.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/grcghfajn.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnafnomwa.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrxdoqdj.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gpvrzcjzf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrkaswra.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gqffehiam.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjaspfupe.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqevzvcw.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gnwlwqocm.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gaepgyjox.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnmgzaxhz.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/grcadtoaa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuwoijaw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gypitblcv.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grgbytvov.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxclinksd.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrzrxbfp.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gysgjvyjl.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnzutdyl.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyvvwzqw.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/glmrjzvqp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlwotvpq.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbfhgiqm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjihusio.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gubglhzmr.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gquyxvggh.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzsptauo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gvgbmwfrw.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmttsyyi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/ggtviyeko.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxrafcco.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gxqgbhncy.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gpvqdisii.sHtML


<!-- 参考信息 -->