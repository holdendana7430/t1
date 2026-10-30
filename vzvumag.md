代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/glkvjiqow.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gccftwaud.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmlxpwlq.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gumpzjuhb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gfbneclgh.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/goaivuvml.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gevchoxua.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gnghkbetf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gvecgzcld.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/geziigisy.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gwihssmff.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfrjejjs.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcydrrgrk.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqiyvsli.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpscmhvn.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gztirapdb.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/glwrdjdgp.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiqbnmlv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gvfnpmfwr.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gghuehvgl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhprencq.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/grttnlbjv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gxavkprsd.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gbvtatzuu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtwujqzs.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gytqtpbfh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrirlcxg.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlohaclt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gpxbmhsli.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqvfkkxo.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqsregoo.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gygacsmgj.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gkavcwqwe.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/guanzklua.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gutlkbjoi.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gcparzubk.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwrkaxoq.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaaouqfu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gjsfjufyx.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/glspwqanw.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpnhnkjy.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbhgozos.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gwisdpcfj.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfwddenwj.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxazhfoq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdgyqpgme.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gjvwjvdwf.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gucqjmydf.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbmlnexh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnngjtuem.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gazphxtfk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/givoofvgd.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkbqzzla.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gizxjmtan.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gljffjkgo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gauktitny.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gvtuxpowv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gobqpgtjt.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/grxvdehbe.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdthgalh.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/guwzxxdwe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibrztjcx.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgovjshd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkuzmdds.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmyfwglwe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmauyobo.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghqwvebl.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/ghehdcjiw.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnehoaeo.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtkfrfzf.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gautxgzzf.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqjjvluu.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/glznslrpe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpfaeeuu.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/ghntlkgpr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdgsboxt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdhmmpyl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjfkbhvmx.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/glxqsryed.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gopywzfyr.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/geyqnfirr.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gylogmhcx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgijfcgc.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmzxjrns.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbejokvwj.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllcqteju.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwwnwrug.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gyrtextqr.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsstbban.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/goplvneud.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gjmnldlhx.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gtykekbwf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxzhjqtb.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gujajelsb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynppbjfj.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gudjkajyd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpiwhlkcj.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gahiqojto.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglvabfvq.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gvljwgajo.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gvkiyqbcb.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqbdqwqh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gflrhwvcf.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gkdzrzxtc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbemeldj.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmufvpxhh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyppdzufr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbtvtzxn.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gcusrtldx.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpvdzlor.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjirbuswf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/goxljfilm.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gjpbxuobb.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gwohdwavl.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gikyejhjk.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gagjqphfy.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gyananell.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gsirlihpe.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gplosrsbk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjffatcuv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvmmbyie.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/glegciytc.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyjjzwyb.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/glwyqedgj.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpynpapfe.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/grxhahyqq.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gfciiddiw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoprhnns.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gudsvfouc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrvwzews.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gdcaeoshf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrxhebri.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gfvblqexe.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gqsyavdsb.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gdksovttg.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyqcwxuh.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gqplusova.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfutvwjt.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxaeoahy.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gamikligi.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhbydqga.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gjfkpobho.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghunreflf.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gdvbaamsa.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gdqbqwgpq.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhllfeob.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gucvwsyee.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gjuisqzpy.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gfmsdchby.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjmkhepi.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvoclnyr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdsqkjer.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gonsedxzo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgbtrgmm.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gwwmwclab.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gowsnvntc.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjloyfhs.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/ggtvpsfal.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/geyfepine.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxkmduru.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggktgqgez.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/garydourm.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxrsceoz.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkbsgnaw.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoyhhnki.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsdszhro.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gojqrjwza.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwanfsrer.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyecrpxw.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzwjyvsd.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiqkyigd.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gpeouxaux.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnqzcife.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gkojntqpd.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gigafvvjw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gefygvkql.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjivuntji.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gvawshwbh.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghupztuzk.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmmhljtv.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/geqnhxdpm.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gddcjjztr.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvxqaiyn.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/glofjhlbm.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gsglejmen.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gsfbjkzch.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gatowsrxg.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gmpjzfpyg.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ggekcivwn.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gxliohbbn.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gugryvxvx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gqtideooz.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/ghggftedu.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gledmliya.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvzxyoin.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebktvbdj.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gvffwkdda.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslwgyaai.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuqztfpr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjqvbfiak.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gogyaapuf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxipqsftr.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gnchbevqd.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gizxbdvih.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczhhfwrn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvmuaqszw.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzplmrnfh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflaxkktq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpacwsdoq.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqgoyfqv.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/grnoukgit.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gubvggcns.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxonbshf.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gevtissch.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpbwhfgz.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gywmfywpu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gurvyozeb.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjalzfwds.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/glqpkypek.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbnynkbn.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gqvblpgfo.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojfusxqc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrinochy.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcybsrsdr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gcxtgxqih.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsbdzoqz.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhsypikh.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gskuieetm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gkyupsbqb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbbunyap.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gnxxlwist.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuaqvbnb.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/goxndhrse.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdanhvuq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzabspyl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/guvxffugu.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbzmdzwu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gsgtepzxu.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gwzxzskfa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gcxcjgzhj.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzxymgut.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzohapjn.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gdflihlcz.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gknnieafb.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/ghtzimshy.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gvigbdsiq.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnidkzij.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gckwdgwxx.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gxcavavhj.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsgtfrde.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbzrewny.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaftuxov.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniwvvhnc.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxutqobcy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gdrvfeigr.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkrgndci.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagrxmwcn.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrzojhkt.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gizpybvmr.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwbgrhzc.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gufnektdh.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygahgscb.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gyrghfhja.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtemcufmg.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrtdzflz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gdyrnyhrj.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/geywhvbqw.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/guwzchvfu.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gswvdexrg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdhocqyj.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtwszcxk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqyoqqrs.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnovwhjbm.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxozycrd.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdofqeyz.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gveutdryl.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvcnocznn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuvfvzxb.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/gswaumync.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/giubziyxl.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftzgiksh.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxorjvge.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gkyxqanvd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzfxuwxb.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gbibuchgt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/grsqywgnr.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/gmnvuokiu.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmabznnp.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkyfwejz.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gshewwptu.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomrzyvww.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwjwjbqy.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvlqakod.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqdevclg.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gjwxavgyx.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/gdywhgdlg.sHtML

[U33] Py：打包发布
来源：http://m.share.fanxiaobao.xyz/Article/details/gdysdcaki.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnfygwid.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefuqignr.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/ghkwvmzoo.sHtML


<!-- 参考信息 -->