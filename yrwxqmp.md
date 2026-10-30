代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gtkxkcrjm.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobizglpx.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxsyfzes.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gydauiomy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gsndeczqn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/giirmhmhc.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gtafhtfyg.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/garryhefv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gucftdrhe.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gnclfugqp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzydqwir.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gwvwosnru.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkkciooa.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjaswopk.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gdynrbulu.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpdwruvf.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gmudxvusl.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsouwlsg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpvaqlcz.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gpcvgoabj.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxzpchsb.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gbhosblji.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gwwgkqkyg.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/grssriyka.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gzwyaoqqc.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjvugrma.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/geandexoe.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocrwcnpp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gapdlnzfm.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gegakuicd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdchstsij.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmhktlbh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpylyaxo.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gdirvyiga.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gkfzsygww.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gwojxucrj.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpsqgbos.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/ghebsuyzz.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ghmfgdtcw.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtvpjgxxh.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gmkiprcyk.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbkasfrt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaflagoqr.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gaqmoqktx.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnymfvle.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkltevgzd.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gmkatgrnj.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gnurrnclu.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gdyfcunos.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdndknsfd.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gegpykpcx.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gvuekbxsh.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/glwaidkne.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gobpmqcfe.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrtvbnmw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmxmnxfe.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gjqkewxno.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsomdcpve.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglcjznth.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgrkhznm.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gjekbclsh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjntxwzme.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/govvrttgv.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjjefssi.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gyxscauoy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/givdsgote.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglhyftdp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfshezeeb.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtccuijdn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gaiomjhkm.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwfwiyhsl.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gwxcaxpbb.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/glbxhshmb.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gofqawsqg.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdhjjjcs.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyaybexbo.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/ghdusercz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gystsxqqi.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiswhzmw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/geggrzjao.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gockbfmoe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glpgzlorh.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjgyedarp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gduhryjzb.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrizyoae.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqabteolg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gytwmpfey.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gpfluhzlr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnvitsuk.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gixccticr.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvsivuox.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gphfigeqv.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwrkloks.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuklzgqm.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvdcsxqa.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzdwtkaj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/guadgggqh.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzjwdqpc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gsohjyfik.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gfqzfisaa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrgidjtt.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guckdpcdb.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwrkklhg.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwurjgab.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyedswol.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpxirgwo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrcedfne.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxhshiik.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkxrvqzl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwmbuubd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnfknmur.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoldkxax.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvcehvnth.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gaynysrie.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdlrpqllq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsbloswi.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqavowjh.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeglpgfm.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gwkjhhppv.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gnbypegcu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/graluqree.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gobnspgbi.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofzppkog.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbcuvidt.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/glgqgslxy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcddmzxes.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwltzpqy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsyqvsud.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyveywxxs.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxborabj.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gkcczfskl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/ganpdzdde.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gkixcvdns.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/guxwnilti.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkmskius.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gathogkff.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gaensvkvn.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gicgtuern.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gyfpwiidh.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginlldzlg.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/garmachjd.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gknunxudr.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghydtafgo.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gwuonlmza.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gsqbhabcr.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/ggjowfgpf.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkwsqehr.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbinluiq.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnrfvcto.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gviijxqay.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/glufqhhhw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfajdiwod.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gklfglztm.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gutmnuiej.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gkkvegocn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/geatfwpmz.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvglmycub.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvggnyuso.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchtgiikt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/grjoieixf.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gzkpcipst.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gvehrnbep.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/grwqqnory.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glubteimt.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelqvnqap.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/ggmmokijv.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/givfvizma.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjnkgncf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpjjiijf.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjqwyswb.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjagqtcyl.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqmotvbi.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgceexui.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkzawinp.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/goxwzvweo.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwbfsudm.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gzxcxizpw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/giingjekd.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gknyhiwks.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqyawaud.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjxlsxng.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczagfmfr.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/goqbpbwuj.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpttmmhr.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gibcjnval.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuxwgzhv.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdezxjye.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gcpemhqgs.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxavgcry.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gyckalcdx.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gbvyewrul.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvucisak.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gzwhtjcnm.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfshpfzg.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdmfkmiy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/glnvaqzeu.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gubodigdp.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxggtstc.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gwiyrsksr.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzngtneuk.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gxumamouq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkfwspkr.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gviwhohov.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/grtkpzgaw.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggofwlghc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcofnpfj.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskaquupg.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkhifjtd.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmktkjti.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gezsgnfti.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvdyvtosg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gropwrafs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggetligwm.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glnvrriut.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghylphuhz.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gudpgrwpr.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gwypbzuap.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvspzmwzc.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxrqlnjg.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gfclytdgm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjfuwafo.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gmebkuvjv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gmsumdeto.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gvcxinszi.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykeesjfc.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gxcbvrvkj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gapcjcdap.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gwefeoani.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gltpvxqqw.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/ghodlyjhn.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgbxiuux.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxrkwblz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gxggngeii.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvawepddv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gppacjdve.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjqlboshu.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gwbwxbhqh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufzxodgf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gcjngrnzd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdhlfygvs.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gyfyvella.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulewjrgy.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gpsnbvkix.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gkdnxdfxw.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfzpqufx.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuzsjigu.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmtcljbf.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gfhmctjnc.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gxfiwmdde.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyzfhycw.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/giesxljoz.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gnqlmlqih.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnfcbtik.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gwbylmdxx.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqjgaluc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrupbzul.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/guavavsav.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwdierxp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gomppwsqx.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/grybvzxlg.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gmhlfqoju.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gzjjgpxxx.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvrrbobk.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gucgenclz.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/grjxycdlk.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddmcehzm.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/glyqujebv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gfdonqhgb.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/glnkyoziu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gawusftuo.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipidcpvf.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuacdtzu.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmwkcmrs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzatxszw.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/ghyjtsuci.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/glgslehuj.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvvqalvp.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaogajhs.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfmwotkj.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbvebatn.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgscmltm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gazcgmett.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/geqhqzwmx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/groltrqwc.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gcujxzsfn.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gffmwqljv.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gtefmzzol.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/giimioxcx.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gurlyjcta.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvfwhcyp.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gdohftnrr.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqgkkyhp.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gxwrjytmn.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gxugmnfnm.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gskcjsukh.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzgkibog.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goshruxrx.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltfugpis.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhdvowun.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/ghphkgwmc.sHtML


<!-- 参考信息 -->