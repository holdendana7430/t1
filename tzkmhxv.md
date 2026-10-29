代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gokdafsyu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gaxwlxexp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gsfxlysjf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gdykyfnni.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gekmcwhfg.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gwugqbkoi.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gdrdllbww.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gssbjhqwf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gecppeqer.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/genwwocug.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gwshycjwe.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gjxrqvdxs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gpujzcsvu.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gkitodgrv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gwzzqqmcb.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/grvhkgjbt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/glnwjhfya.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gqfezedmk.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/govocnwae.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gjokzvtdx.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gtnzztcnd.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gjiyhysyd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/grqsljiyu.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gmlfmpflg.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gtadxptxv.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gclvtofyq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gboxucecc.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gvdeekzuv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gslgxyscc.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/ghpticbys.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gefqzzgzn.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gfwbulren.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gcublqcil.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gdpvrrnju.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gctuwyeyu.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gbtstubbo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/ghxtzahpb.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gcblgwyur.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gngfvphpw.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gcxwpidde.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/ggjzbhrxn.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/glennxkij.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gidhaptie.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gamglivom.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/goprurrwh.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gwmrtkgrg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gmenkbabu.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gokgrjsjp.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gwczjmmss.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gvbpkrlsi.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gdnegupms.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gfypvflvy.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gosguqech.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gwdhmyiri.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/guyhohgbb.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gebotmehu.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gisrzyula.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/guchxcsbf.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gyxrwmefx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/ghaqicewk.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/glfxfgtfp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gxzdwxuah.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gijbhqwbl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/geupevwpi.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gczwnsfhm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/guaupmisk.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gkaneizkk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gkumnvvcl.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gzxskukam.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gzzduglnf.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/grryedqsv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gbzxpnzqg.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gzgcrslib.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gewhugmkb.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gseknuqin.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gtpccxgnw.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gxnauoeil.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gsvhrujzu.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gwblqlpjc.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gyruobztj.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/grfbgkquu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gvlycfjeh.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gnwzlavgn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gdgvpubks.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/ghenwtzav.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gsxywsvvw.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gbetdyowi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gtnuollgi.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gygpgzvtz.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gedshhysj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gxtcrxgva.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gtgnygydb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gxnjcxhvb.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gopbzqxwb.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gnnufrsgn.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/ggdlgswct.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gvkkbqgel.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gxlrxfvuh.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gyatalorf.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gzibiswqy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gsuvwpmcd.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gjggastvr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gmmukhrav.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/glodfxdif.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gbriegzkh.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gedaklyvz.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/glmtujsus.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gtliljahd.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gehsvxujz.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gnseidboi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gjrfbdxxt.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gccvtupwf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gopokmkqb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gklzqjter.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gaouyyafy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkeomblas.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/goqwvsiac.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gpcpyrldm.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/govnspdap.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gabkswlet.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gzaugjepm.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gqahbsjqv.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gansylfvg.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/geixtkguy.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gltaehaaw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/giiegxivm.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gygczfqus.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gaoymtixy.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gzsjihuvn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/glvnlogux.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/grwjjyycu.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gwminjapf.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gzruojngl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gjbugwjsa.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gstubjovj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gpixgpens.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gblpzqjva.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gfrdkpejg.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/glucmykez.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gprpzbejf.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gyiwovpte.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gprtwregc.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gewehxvnp.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gmaadxcbm.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gtzdumnto.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gtnlnhbsd.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gclnkiaeq.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/giivezoxa.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gzkprrtcw.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/guxgfzkqs.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/goasjogta.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gkpaafgfe.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gwpapgewk.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gliwfvgkl.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gzizzgpwu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gpaaporey.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gwvagpqxe.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/glhoznliq.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gprplmpbg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/ghnpqfiir.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gqprfznnv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gxgbdekvw.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gsjrmoiwa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gasqpeywh.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gfzwfsivs.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/grumuvlki.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/ghqswehfp.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gymoczzpq.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gmnmhgrtj.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/ghdrcpsfd.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gcevkrjoj.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gvxwjjzid.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gvrwcrtcu.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gxivltcuz.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gwcgicpcg.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gctjbzpcx.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gjtgqpiae.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gkdueceal.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gwnrltgpw.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gahdgyqeb.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/getepixuo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/gdkhtzcab.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gcbjqhfwv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gfropjwrq.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gtwmrtrgc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gyzezsuwm.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gbcxdhzmp.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gayqjsxcl.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/govvrjcju.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/ggtlefafs.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gcmcuwyie.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gqvtanqdz.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gollrlsqn.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gudrkcite.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gvwkfjupi.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gwgrjetno.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gmswizppk.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gztnlgkkf.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gvidrrrqp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gofpelwzq.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gjjbvgagq.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gqqqshiem.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gotdkvsee.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/grogmzwsl.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gbisvlncl.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gdbhmyltb.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/ghsehlwwi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gnsfbsgfm.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gqpiqhoxu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gonwppzmd.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gtahlqtbf.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gvrijxuzj.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/glyxaybdu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/ghevgceme.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqivzpqzz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/giqjtdevd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gfetwiucu.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gkykgqpfw.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/grtvlbpeo.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gbpmnamxn.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gnohuqusf.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gttzbmjbk.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gcekdahll.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/ghrpgftac.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gxexgwuki.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gygbcjtvl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gqmwwpbhg.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gtgvbxnds.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gjixkwsxb.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gfwnuoafn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gjgqcrisn.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gflcewvbt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gqomrdazv.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/grlvmkkfx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/geecuzjbg.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gamqulfte.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gtqpgtffz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gamnremvx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/ggvorzdgd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxefsqmhh.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gwjlwgejs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gakfdhwvi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gkvesmhvc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gznheoqdt.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/grqnommds.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gbtxtoupl.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gttayfjss.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gnqxrmvic.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gzndkqpsd.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gyrrdbvyd.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gpzxtxwmd.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gcbkvipmp.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/giwounbtz.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gzfprgizm.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gzhspijle.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gogzdalxe.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/ggzfgdopi.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gxpsbfebk.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gdfkhpeld.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gpmipnmbu.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gntspnchi.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gbmilpigb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gtahgkgto.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gnfmoljfj.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gjsijftlk.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gdkmfapnt.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gkemjdoch.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gquxoxxuk.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/geerzxhis.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gyxooevbg.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gdfmnqjqi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gasmqcfxq.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gwkvpwxlh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gzaahctol.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gyvqlakct.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gnmebquhj.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gheuwuvqo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/goyqustrh.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gmzioxcpc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gacyxuofj.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gvpytkjtm.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gkzrqxjfa.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gbqfydart.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gwfabszib.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gcghajrco.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gcrxezxqy.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gqvsmzoti.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gozqyuklg.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gvhvyjyjn.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gxokejxkk.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gjcpxifnk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gdgwffnnl.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gabisncyf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gjmlnddnk.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gshgmedpb.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gljrxzxqe.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gqmknqmbe.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gnldlzslt.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gihzamnhm.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gwdekyija.sHtML


<!-- 参考信息 -->