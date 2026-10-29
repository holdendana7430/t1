代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gnwjltriq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gfygrupla.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/givavhkjo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gndybhobz.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gxqrkonyg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjkstprud.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gmvenkgty.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gbkagtgyr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gwcjypnio.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gkntpxjej.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gsqvggdoy.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gmpchygnk.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gyddmfuju.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gsfdyjyws.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gsdkevekz.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gxqdxycgu.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghuqsyggv.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gojakghke.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gregcrmcw.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gqpezlemk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gsjlpxgxm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gctjymdxy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gomntzfog.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/guxdcdyho.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gezyyfahg.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gremwokkv.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gryeoxnwz.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/ghrwducua.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gwpeczmhn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/giyinffia.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gukpofori.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gkxyzmgwc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gsodpdhog.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gzsruglzi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gzqalwcbx.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gygqykfav.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gkthlnvvg.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gdurilgfb.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gafcajgwe.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/guaadgsgu.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/ggtvxzftj.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gqrimyvft.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gkndwecsr.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gvvmcxtud.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gqkhuuwxj.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gtlwxhmuu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gyecricdy.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gtaxcvyul.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gseukgoph.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gvubxlrxc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gpkeidbqy.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gdpettgji.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gcnapaxgf.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gwlfvyypx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gxazsicgp.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gjcztzjol.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/ggdjzodxo.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/goiesaboh.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gpqqujfjd.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gixocfjar.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gtqtiikzq.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/glwxrjgkd.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/glgiunbnf.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/guunbflrd.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gsizzxmxh.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gdosbolem.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gspsohelu.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/grqnnkfkj.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gnjxvlgio.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gwacvklyk.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gufavtvnz.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/grhxjiihc.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gykxwwwtq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gdimevauk.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gceukfzxi.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/giyuaccce.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gtjadsvrm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gbzesuobx.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gidfbzjsq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gulhnuivy.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gtbapseqj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gkmkhhqzp.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gozwzkawj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gupgsiysz.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gscchhano.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gzxqfdrpw.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gywnaadtq.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/godcpfrbp.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gkqzodaxy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gsiatkpfx.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gkfbzexcj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gyqaqqgjd.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gtgdmilmn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gwhpympnk.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gqbjqhezb.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gtwkaufgx.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/ghuzejwwq.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gdjqpnqjl.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gaovqootb.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gsihsuiyj.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gdmlbopdn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gbjygxvkk.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gykuzbjxa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gbnfiqlce.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/guzgmynxn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gmkmbpqvz.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/ggxxlowku.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/govjauunl.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gqmfvhrkn.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/ghhpdigod.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/guhpgijwr.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gwjhsvoip.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gzhnsszkv.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gvyjgmyel.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/ggojaxosb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gkqeqvtyy.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gzxdebtff.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/guxktsyve.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/glucksysd.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/grlotpfpa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/ggkfgynmf.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gfpvzfezu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gajbekkin.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gmwdyagez.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/govhnjiqg.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gqiijkpab.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gjajtjyzi.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gaimflvym.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/guarvuyps.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gscpsftdo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/grzxxadhe.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/giazzgage.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gjcoxuzfw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcjugxwzu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gdpyqsvtj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwraofasy.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gwctwvcdw.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gegexemhn.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gimqufbgs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gksxyprpp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/grgxjewhz.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gyrystfke.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gxbjjprkv.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gdgqhsdyd.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gjtshssdb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gutjuurii.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gflotdzpy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/ggthikgot.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gtnbdhluq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gxdljsaad.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/ggqobnhvu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gxaqriwwg.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gbzrjvrud.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gvqcfgtaj.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gophgovab.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/graxkovih.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gjlkotmwv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gdkykneqf.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gagqzkokr.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gfsqvzhrm.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/ghbkrxnnd.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gxqdcpjzv.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gjwtjpmrs.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gtdahyllt.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gxewhksif.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gpesxzgfr.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/genereddh.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/godgkmjai.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gawokzixj.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gjiponzqo.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gbjharpxu.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gfbmiylup.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gjrdxkthx.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/grngiyzmg.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/glahkwwtw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gjliaazjw.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gijeicwhy.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gptnreqdq.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gqqchuvei.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gwmhmhncw.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gyhcxdkuz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gugryretv.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gaterutrs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/ggjtotgbm.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/ghprzqekj.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/golqttmfa.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gnudnowkd.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gruhohsbf.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gjbmstwca.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gfnmzfatn.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gubxqpxgs.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gozylttau.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gklsfppxt.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gwwtoczzl.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gbaijqpod.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gwpiuekbb.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gequsdluv.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gcouwyaex.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/giikgjlzl.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/gbenptdyp.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/ggcqpbvhg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/geglwwsmk.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gfemptcfb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gkbauujxc.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gtjlizkbq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gfablzlkk.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmubxficg.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gyzpibdso.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gouwvnhao.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gmzskbpqi.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gexnqexba.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gsocewiph.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/grpbhrben.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gicbkacqz.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gwnescirq.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gtcqxbrye.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gtqnizvoj.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gxinohpqi.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gjmnuqohy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gzniwdpqr.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/glavvnauz.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gvkchxeic.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gpykrjdgo.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gkdrwxkkg.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gbwafyttb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gmzvnidqi.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gfmluxqfo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gzkpnnqyu.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gxmvkrchp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gznvkmgai.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gdwvemyul.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/ggxuycfkk.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/ghzycctic.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/grifldskg.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gleubkuta.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/grlsqgozj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gfdpchtkt.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gqoxroqmm.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gbxtmabei.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/guaobssuq.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gjjjqaywc.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gxbqtpfyh.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gqajgwdve.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gdrbzgpgz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gtcywjyqz.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/ghceksrup.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/grzdmgugp.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/glojantow.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gyuevbjqs.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/ghntsgjlh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gnpqonivt.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gvnhugqwd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/garnccvev.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gmabfmzmj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gusyuxvsv.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gdogjqksf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gkwxmiymh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxipqihtb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gxqqoufgy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guobpqhno.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gulmwjird.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gwizutbju.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/ghwshzxue.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gvcfmnbvb.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gghfgwsyn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gfcmqvsju.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gdfyuptgx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/geypdqjnf.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gjzpcxkhw.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gyoodhwti.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gystvieqt.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/godgmrcly.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gljsyiplm.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gtnzqzmhe.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gcdkiepcs.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/guhfyfbhs.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gyaarylfz.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/giatowbvz.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gxathhwbi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gfwtotbbq.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gnceowrzb.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gaebrayuf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gbvpxxxsb.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/guzxsbnsc.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/glvzyvdzg.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gcnvkiawj.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gqqogjphj.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gbezwwkgm.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/grmnxwnqt.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gugaeltau.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gcojqzdds.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gjgnutsnj.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gqbsndofy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/gagasqcvg.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gowahebms.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gzrzcajig.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gvkagzfqg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gpikcwdxh.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/gtcitvkjd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gfihxnszz.sHtML


<!-- 参考信息 -->