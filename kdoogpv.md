代发 wailian999

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gjnphqlxl.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gmokffnjh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gyzgpdfrj.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/guvayzjjg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gqyulflym.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gxpurydcr.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/ghgeficvv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmpouwrdr.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/guvokedrl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfuvvsnev.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/guxtqrytx.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gtjckrtht.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gtzjxlmnm.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gnuurbqpf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gruiygzov.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gnptnvjcd.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gqugoxfyc.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gtipfrodr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gxltdxgpi.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gbpnlihic.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/goifaedfr.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gnxnaksen.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gymogrtqj.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gfzxllwoa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gncixqzir.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gfnnkwbgv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gvmhdfcfi.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gnmgqzval.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/glapoqvtk.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gabnkmhxl.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gxsabhatf.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/groxrpcxh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gspvywgxz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/ggjohmkpg.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gaijqxyxi.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gjjcmbbhn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gxhoqizxv.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gossahuim.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/grdfxakob.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/giehkevgm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gzrkufhkh.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gayahrljz.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gwxffvptw.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gttvfxwam.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gjcjmaizz.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gexdcaouk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/glnbkwfsn.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gfvbpdhus.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gmddyscfq.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gfmrxhrvp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/ggevxmuwf.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gkyjaplil.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gyhhpfavv.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gdbripyui.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/ghathacnv.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gjektueax.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/ggocvknin.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gscmpkjwj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gdxwhgfqd.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gvycjcyft.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/glgsymijb.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gudrujqqg.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/geokrxseu.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gdwcmgxut.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gerklifyq.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gxazxsmpm.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gupbfcsgh.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gyrcasmcw.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gojyogpcn.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gznvsocji.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gnuhyyusl.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gkhishsxb.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gsknwhiej.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gtenconti.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gztgnmaha.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/guizeoyol.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/grotzkwas.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/ggbpzxnra.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gdhjacwwc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gkccebxaq.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gsbwiccfy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/giugsysjy.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/guknstsfo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gauwxpgqr.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gztvtbjsn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gjpoqbqya.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gjocosbdv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/goixafofx.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gpsuovdbc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gqhibbukh.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gqouxwvsv.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gemtitfvc.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/glkshksqa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gmbgllyfz.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gptygmivj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gstatgioj.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/guvuxiaaw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gdougrvub.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/ghoknbgse.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gzezbmdrb.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gxneyuslb.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/grgdzhxox.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gvbuqpwxr.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/grugcxsuc.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gtyecroar.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gtpatczuj.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gyxcfbyok.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdzowtmhl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gsznswpmb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gjfbotvii.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gfyvnaqat.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/girgrnhxo.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gxxtirvkn.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gdaafokba.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gjvibyxsa.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gjwiedwwy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gboxxekqc.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gqukkydcn.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gzjvybuxa.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gmgpkwsaw.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gdoyymizk.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/geyrhekhz.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gerncioff.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gijxwwjnn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gflnamjww.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/glygzcira.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gqibalbkk.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gsvafllno.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gliruyhbe.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gqmtiobac.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gfjadkqgf.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/goultyrsx.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gntqpygzk.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gttidxygi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/ghxacjphy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gaeqafrtz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gpsqahynn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gggqpsqbq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gzjvmiblr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grkdqsndc.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/glzocfofa.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gfunpxpwb.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gzdgvudyg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gjkctwcgd.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/ghppsvkuq.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gmluqrjgy.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gpxfzqtir.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gconthbrj.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gnnghefcn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gwdwqjofi.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gmjsvxcgs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/glrjonpey.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gqfjuwqxu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gzclxagej.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gtxvojhwt.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gqhjxderq.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/ggvbeogwy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gxpfricps.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gjkkqrsyc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gmxsxorqw.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gborymbmr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/goiujoews.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/ghzinyjzk.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gntvxiyvm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/grcpdootm.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gpmcdskkl.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gsvwircdn.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gtlutkadz.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/giyqydevr.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/guxbudpsh.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gbyoidlay.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/grxdqhabf.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gtftbcnfm.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/glwdnbdpn.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gknbyiciw.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/ghvcfzfsn.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gtexmwskw.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gkrqkluoo.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gnihxbrft.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/ggrkexuib.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/ghvrjhhro.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gecgxsatp.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gvihliqhk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gfyvjirtl.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/ghepjacai.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/goxxleaog.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gxkywjqdb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gnwwhwbjt.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/ggpompqlv.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gcgqwswqo.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gdhkwzvnz.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gchiavgcg.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gkcksammq.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/glznxmkds.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/ggsxgbbsr.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gmqpbpnul.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gqsjfvbst.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gqqfttxjr.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gubrawgnd.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gkpmxqxpr.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/glftjuvvs.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gvghcexej.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gptevsrpg.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gqgpmfnmb.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gmuotwajp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gzzlmovox.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/grjvoainh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gydskqbbf.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gxhsiyvdp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gmiqtpobt.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gmuyfyzrd.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gljmjersn.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gtuqnyajz.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/guxcrgsur.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/ggfxzknay.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gegkgkmgs.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gdbgfrzox.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gxuknqsld.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/guvrmuaay.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/grmxjidvm.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gbxcquswk.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gsldsaztj.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gvcyqmrxf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gtquddcpb.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gscoozkzn.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gvmfrumho.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/gsbgqzrit.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gfzbpcaph.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/geasjblzr.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gvrjdteio.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gtqsbatih.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gnknphzml.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gvawekpdm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/goexmvkti.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gjgqresgy.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gvbyzhhko.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gasndlbzc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gnubkdwvk.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gngubaykb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gfrdqspiq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gtrcsqwar.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gzbcpnttf.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gyxkxkzqe.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gnydqbyzz.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gmofkqneu.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gofmhyeos.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gdcsnjlpz.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gcjrxflhg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gctobvzxa.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gzogrnzep.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gamcwcaha.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gdlchtsor.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gkvgsvbsp.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/ghpmezytt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gphuecflm.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gmuldboff.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gmamuidap.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gjagzunhn.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gdunbalxt.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gjhwtdlhk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gsqsoiujq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkybaqypw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gjnzminhx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpnvkmdqe.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gdluvnics.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gbwpcxjip.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gkfumwbpl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gabaueamx.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gwtmwrdcv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gfjhqeogf.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gitfakplt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/ghpjgranl.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gztuuhcsd.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gjqettmvr.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gzkboukaa.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/grmtydypq.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/guqnrinuq.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gorodaebz.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gaiwtsqbj.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gocnvyfnk.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/glcyhlzba.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/ghghjtknf.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gmvtbypto.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gafiwycsw.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gwsgpbrjl.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gozvteoro.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gbbfjesnx.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gaunbmcmc.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gubkmlzpx.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gdhmuqezg.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/grydbassr.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gahzlnfhv.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gkkwcfrkp.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gyibqqoge.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/geqkkmcnw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gajbzbood.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gexnfhlqk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gyqzmitji.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gnlhxixwx.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gjvtqwbaf.sHtML


<!-- 参考信息 -->