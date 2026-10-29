代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/grocvczmq.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gcliwnbpw.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/grbvhufie.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gmqcqouod.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gbuipwvtl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gmudmadkd.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gfarxklun.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gpawhyain.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/godfztdxl.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gmjjpteea.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gbddzznpx.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gdzothrdf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gftgipwll.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gluhyockm.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gozoylbeh.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gfcrkchkr.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/ghmrocxpu.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gagrprffj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gdlbvqwhw.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/geirxoapm.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gwwfwjnaq.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gdgoxywia.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/grrxkfslf.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gtwimcqpb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gwptxhzun.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gvpkyofuo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gychpqkyl.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/ghxmlzywn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gkktdgeru.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gjxakdvmu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gbqfuqaro.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gfcknbope.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gpiqdhscw.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gfnfzryil.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gxqmfkynw.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gkebqxksm.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/guclmncpw.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gwffkwlqs.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gmyrxqdlf.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gxzbjrljy.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gcdrgapdr.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gzpjhzmsi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gkauuojti.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gkarbjnyb.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gmwfaxenu.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gmndlnfhz.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gdcwusyzp.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/golhjhvhl.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gqxedtmef.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gyiqjizxi.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gladfywpd.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/goxhcckhq.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gwkptrfcz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gzbayhoxr.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gtrnqruke.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gbyshmlrx.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gmwmmdfql.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gyvottlua.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gongvrzlb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gslhllirn.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gzfzydrrs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gplthxkpm.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gzzlvjvez.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gcodrwocn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gmerdczxp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gkqvssffy.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gkaizonac.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gvewquuho.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gxrhvchyu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gcrdgehyy.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gsmeicriw.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gtmrvlzoh.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gyzzlufju.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gvvyokaic.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gmdgglhab.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gcznqkkts.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gowpwmjrq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gqjtkcwmv.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gxljynipg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghtjvovpl.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gprlahsun.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gyqfwbgsl.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/ghuhejcwb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gbmwuxopq.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gstyirmef.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gfpfjwqtb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/ghpxhsihp.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gszpupcjx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gjpjcypqq.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/grchlhsdh.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/goqdiivbb.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gtihyotia.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gtsfcsuvn.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gajvrmqcl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gmteddxhm.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gakfldnfj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gmcocisjv.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gcqahuvxx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gyrbpzypz.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gyrdterci.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gmeqsbwni.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gsqqkvsfb.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gqnhdewde.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gvbhsrgsy.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gwtgplpna.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gbpxarqlw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/ghtnbztko.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gqneiuqko.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gjcgzkdnf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grdctukzy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gdqtccktw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtgwrmzwb.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/grrdccnfd.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gimiqhdxz.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/ghuagopgp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gyopqmtbu.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gavfepwmn.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gxjpfadov.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gyaarxgtm.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gmzcpzdfq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/goewsdvev.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gddpwrkaj.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gffisfjks.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gpylykamk.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gfxxirxgf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gmpdbzmdo.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gvjzmszio.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gjpbsjjjz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gfbdlnotj.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gqliikwmf.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gebdsuntb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gllssckoh.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gzmqotylq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gsfelldqn.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/goojclczo.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gbliztdxp.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/ghffaxiar.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/goqaqhqbl.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gymhhvrxq.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gytulgusl.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gmfibhree.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gkdzlxuxr.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gzmbijhgy.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gjogyihbh.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gblqmfosn.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gozsemoje.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/glutigdvo.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/geoskjfyr.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gpvcudftw.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gfhucxkfw.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gqwbwrpsc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gmidndlvu.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ganhdttvh.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gazdovrne.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gcevinkou.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gnhnoekos.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gemzgwawl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gyjiknene.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gryyfvnkd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gdoefhgkq.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/ghsgrvqni.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gddlivnik.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gkmkveqna.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gydjycjzr.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/genyzwaxr.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gafblxgcx.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gzkevivcy.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/geuokvvwi.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gdcvwoijz.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gzwaubcgb.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gohzqkedc.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gpgfnfrra.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gpptpnxaf.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/glpdbzvne.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gppeziffm.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gltjuxbur.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/ghurfnvtm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gnoeedjas.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gqhksqezb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gchdbdylp.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/ghpygndeq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gpnqpvxrp.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/grfmrspov.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gnhjjaugl.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/geihkynlo.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/glpfnmsnh.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/glrfgviho.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/ghqtzcbuu.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gffqxnagu.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gkwnnvqng.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gzdqjjibo.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gfpgjlcid.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/glopunpmm.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/ggexnywar.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvhxulmti.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gvaykzfeh.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/glwfqbftr.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gngfaouqy.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gxjorlsfv.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gsivpumws.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/glbjzwikd.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gxmbgfgpj.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gmvuhjxxb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gxisbegtm.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gezgldaqx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/ggsdfjrdf.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gcdesquos.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gshstwomv.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gakdzyiad.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/girozpdke.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gdekoqssf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gzlzzqpfe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gatqkrrwd.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gcpxcrlws.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gbrachwad.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gaeyogwdu.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gjtoisxfx.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gcwpydvld.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/greqsokqy.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gditrrzyr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gitpbozxu.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gfighxrnp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gfyiarrwg.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gaisfotiu.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gffopzvoi.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/girksllim.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gdzrwsnzh.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gynqabwiv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gsedgatdi.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gzbgznpvm.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gcapvffhf.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gyillbwne.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gwfsrfjqk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkkvwghiy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gnolvwiwe.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsoqltuis.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gcfbtczzs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gkqkfkhwa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gitikzvaw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gofhlgmfn.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gbuwzelfz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gfemcsdhb.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gpkgzvwww.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gcnnzuzsn.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gjiotqmce.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/ghjtdmwyo.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gycwmszzz.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gtzzvxglr.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/ghcbaxcyw.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gfhjgrfjn.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gbvkwrrbz.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gffjnjzgo.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/geyvghfhq.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/guhwpskuc.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gwodixdub.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/ghtukwpbs.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gozsqrelr.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gxxjvknfi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gxxjvhvtq.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/gmdovljpz.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gtpptaybz.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gyqstaysl.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gpluodeye.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gshzdvgcj.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gfmwmltps.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gqmgyfmnr.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gtnqetcan.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/grnhvincr.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gjqqxulqx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/glnfnudag.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/grmltpkpe.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gnufbqwju.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/ghuhgqkxm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gvfeedkge.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gxnldvzkw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gydpunpcr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/guppeyozh.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gzwbaktya.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gzxjzxjyg.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gvnponpmg.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/giqqfxhce.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gruteukiq.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gmrywzvgj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gnhogyevz.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/ggavoxzrl.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gvdzmavmp.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gkokxjdpo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gzfkglqik.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gdzckqrpc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/goglcoedo.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gwyoxvgzo.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gozwnhmto.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/ghbqoosjf.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gxjxmrsrk.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gojvvxzwu.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gurramxen.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gwaunsfxb.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gvawhjuua.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gktzcwyia.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gqgipynye.sHtML


<!-- 参考信息 -->