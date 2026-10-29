代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gpqwvwvoc.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/goguxtzyb.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/giwhxtzuk.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/ghexrimbl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gppdfsyml.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/ghxntyqxn.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gkmjiakzi.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gkinhbbjv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gwuosyuci.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gvdgqeznv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/glkbuoctx.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gopxnqoaq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gpkhdqsxc.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gdtwbuxyi.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gmhygizev.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/ghzveagre.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gioqnkvng.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gvignhzqb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gvfryowsa.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gnmykfoli.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gnbjkahxl.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gtbabzokl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/getxniztl.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gozfagtcv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gjlackmsh.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/ghnzgcbov.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gtoowamdq.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gqnkenvdk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gcqndqsig.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gpbinlnfm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gukorlsod.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/glwfelzqm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gavpahqrl.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gkfixcrwb.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gocnjdhpp.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gtnoikjuf.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/ghbnunioi.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/ggdxcrqyq.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gsgnukdcq.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gmvibhcoo.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gasomtciv.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gamzxiefq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gtmgobboq.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gawlnkutp.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/glefdfvut.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gfhhhsppy.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/godunjqiv.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gtdmaekyr.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gfghbjwbl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gpnzdywda.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gpklldvvk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gzutaelwl.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/ghimjikaq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gmshxjawt.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gxvpksuaw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gkxtayigx.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gztsypvjo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gooflbsus.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gzeitqbao.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/grtgrubfn.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gxcqmympa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gderkoide.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/grirvaqbc.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/ggwstntbw.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gvzhicmut.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gxppnseyx.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gnrnefbzs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gmtecysum.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gxhzgmhqm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gotnutmsh.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gfacytvnz.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gnaurvhkb.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gsugnzbxd.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gnifrhitn.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gyqfhexib.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gzdpcqjcq.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gnflrtuiz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gljyfcjdy.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gkuiaekiu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gehioznzq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gzpitykvs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gqwvscvax.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gvviiaxrm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gzvqvzbkm.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gljytejtt.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gvekdoacy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gshoncluw.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gjactmodr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gqrtvmuyx.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gkxfuffie.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/ggdydfuvd.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/glkkgnxku.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gpxnmrwea.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gmdtsehjr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gehgakocq.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gfclwysmy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gecjxoakx.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/glkamvgqs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/goymsmjfk.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gyjlzqfrq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gttndromr.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gyufsbjid.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gwehterth.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gbwsiggtz.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gwvzftiot.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/ghpgrnmhf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gvmteuosd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gduitgebk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/ghdexuyqz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzzvlouzs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gahvwnpvd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gligzitau.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gzhniobyp.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gyfjqbgkd.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gpfvixbco.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gfoqexpmr.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gozoawlsr.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gakialhiv.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gaqbhkmyf.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/glurhijtn.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gtxhebrcz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/giuylpieu.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/giisojwtq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gszixcnqh.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gymwpkdlw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/grmyidodm.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gqetdkqhn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gjkasqfwr.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gtsryrphi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gsjibyklw.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gskmyydjm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gokdnooeh.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gphrdpjrf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/ghgpqchrg.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gdlflyoft.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/ghskbjyov.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gchvwyyim.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/ggvyvfikg.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gkdzpchlq.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gkzrvpjme.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/ghsrvrelf.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gwrbfxcyt.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gspafqfql.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gksgwxvfd.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/glnqvjnkm.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gupxphnvl.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gekbfmobr.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gwmlkygcc.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gwnnrrlyc.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/grlikdkpp.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gesxxpyya.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gzcncxeif.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gzoxplotg.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/giklehjzh.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gnwwozupc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gbsrocszh.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gkjaxomsu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gnqoovzww.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gmgzuipql.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gavghxlfx.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gehsorfux.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gyynfsnnj.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gjdypbmih.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gmktoqtjz.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/grqhpqlvq.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gmbxfslzb.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gsyuvfjol.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gunompnpn.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gxqyglxkf.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gfzxnikjl.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/ggkdnqaxj.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/ghwawrndi.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gfmiheprf.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gbizdjcwh.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/ghypuqgcn.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gysrysecq.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gaclxbhjh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/ggrfvkoiq.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gqvwmkylp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gdmhbzqqi.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/ginwmiddu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gytzpbsus.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gyjachnfk.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gpbstpgxu.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gfqjvvkhu.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/ganwlbkgx.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/ghzjbgwsh.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gwueiafgw.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gzcevaeiy.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gaehvdndm.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gatvyxpgv.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gkkutcnjx.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/ggehlqzcr.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gtszhegfi.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gthaivwxk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gkwssdrfd.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gcfjygont.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/griyojmnc.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gwwtlgicw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gxybqdmaz.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gfdnbecdv.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gmhutyrxx.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gazydzlyc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gxohdyxqr.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gtqldnoxx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/guoisknqh.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gvmdmiwlq.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gdhikffhh.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gynugxcyy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gxtkfjilt.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/ghrtftkhc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gbrqlmzvm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/giurpnsik.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gpyrrxoej.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gfoeyxqgh.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gwiebbnra.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/glahfmolw.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gelhhhdhn.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gebjcgwcm.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gztychwrc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gttxspdzy.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gcqvztrjp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gcrkehdex.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gyilofhms.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/ggwpttxxe.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/ghfgyyfgb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gvjxrubqt.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gcgorcgwf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gicfutlvk.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gbepwlpkt.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gzntkbkpm.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gdyjcbozq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gncmjhzqc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwldcywrh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gmsebteyr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gleoupfty.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gfjlqanjr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gqmdlppab.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/goqlfbrdr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gbtitymxw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/ggnkuuhcv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gjhtjfmol.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gibtdemoh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gfpdzdorr.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gqzhpfwja.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gbnejxxaw.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/grjmzvomh.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/ghhcffrdk.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gusrbiugs.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gwglatrui.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gjkcqqomk.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gwrpiwvlf.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gydpgchmr.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gnbuuxvoj.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gppdhzamm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gtusnaurw.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gnvncukwj.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gzhfvyesl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gdydjqxdm.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/grqlfhmgc.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gleoicezj.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gdruvlaxh.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/grgnxmlpb.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gqkhdmhwo.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gbwgrbcmu.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gdzvdalcj.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gfdokpldj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gxtwrzkxe.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gxdewtkvj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/glzylxoch.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/ggfpnbqyq.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gyitmipfk.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gtwsfpiot.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gryuhrtsi.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/ggoqhoura.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gyegiwbag.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gwbbgvdvh.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gqaakjors.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/glchuklqn.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gigvqnhmj.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/glszyooxr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/goilpqwas.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/ghuxdhehj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gvrnbhqja.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gxbxolojw.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gzbjmimjg.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/ggqtjceha.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gwurzufvp.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gnqjwxahf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/ggggbqrvu.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/ghvlzcxen.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gakrnquaa.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/gphmcgwve.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gqsddzlkp.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gwpvsphqd.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gaivuqoyz.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gizghdngd.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gozarfgfl.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gllqyjrds.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gyqztqslp.sHtML


<!-- 参考信息 -->