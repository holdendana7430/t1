代发 wailian999

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/ghaltgmkg.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gkkvtmxlv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/ggyjtucrx.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gqgkdvlwt.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gkxhfyqkj.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gpaufxchn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gzlrktmbx.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gghdplyvx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gbywvalpd.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gaqncmtyp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gahfhpknb.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/ghgzufddx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gbntvlxff.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gwegkdhdg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/giblytikt.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gnzbrkkrh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gkbhayidr.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gcsfhwzyw.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gzqjknkzy.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gqnwgxebv.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/ghswqczuj.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gmdkyqkjq.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gevmsizkb.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/govfpmics.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gzhxfnutk.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gkinafsyu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gkjsnecbu.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gudydnbyc.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gusbaicrn.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gvnaagori.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/goaeakvvw.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gsjeijugy.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gifbwfbmv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/ghhmvluml.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gardjpnzy.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gwdthsafn.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gfdyfdtug.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gzxkaihmi.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gxttmsfpq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/geegisrgw.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/ggrbvgbre.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gclnyhdbw.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gsyaoxalm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gtqzyslcx.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/glquiaseb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gvukzatrh.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gevocvkrv.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/glinmuyyd.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/guklaksrn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gzvogwalu.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gjytwctfx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/ggxhbiykf.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/ggiibyydg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gecqoznbx.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gugdewkpd.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/ghwtjfzic.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gxyohmsei.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gygxtwxmv.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gmvimxcuz.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/glpuuavdn.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gkpjoqrdg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/grgxlmlew.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gqlfaprkt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gfukmkpgl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gqseiwpfl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/ghabqkair.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gtjpwylql.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/grsxyrdqv.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gddveuino.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/glfhqwicb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gbezuyrfm.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/ghhiaslld.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gnzkkahdb.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gcvfcspwy.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/ghpixjbwb.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gjckqtcau.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gyadoayjy.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gluedvhch.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gyusjdfnw.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gngtucrfo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gzbvjsiyk.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/guzmozgsa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gkyaabysd.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gvoclcgev.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gspoypjos.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gmvtoktep.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gmzjsxeoi.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/godkijcpq.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gnvrspwbb.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gdsonjyfe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gziyldqju.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gqzvskxui.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gjcjipxre.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtridejlb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gmquvdagu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxpceaevx.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gaafbluxw.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gdjjognzo.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gpcrwvbvd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/grvfecuzo.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gokmntqyu.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gyugnlqdl.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gzegqjeky.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/geqjhbnle.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gsasugohq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/ggwtbsopr.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gvuzbxvlm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gorxenqfq.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gtstklxgb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gcqjqixfz.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gcqgudfvd.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gizgaumwc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gxcwdkzxs.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gfmfjorpg.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gkunyrmyr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gwqozbcau.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gofjjbprr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gdirjpsai.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gwkcqzgrf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/goktjmfsx.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/ghoiargyx.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gbxsogaph.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/girwngigg.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gnmjwptgi.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gfydgchwx.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gzvawswhh.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gjeblrpjm.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/ggbtqdqgr.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gyqgxtmch.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gqzkttgom.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gaszrrubt.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gfmgbtzii.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gyjfkscwu.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gmojnqpha.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gvmopbwmm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gfvzdtwbk.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gitcaozyi.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gcstcfoxk.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gtafbrksp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/ggdewxebz.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gdrdqkrnh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/genxcgdbf.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/grpcnxfve.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gmhroummr.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/grlmlycmt.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gjxfptqvm.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gnnuvzygn.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gkpeuspci.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gzuyynljc.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/ggxiqewht.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gypezljoy.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gvntpthuv.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gtybqsshr.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gkosyzioo.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gjuzdzvip.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/guiuluvik.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gtvctwmdu.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gdhtdvpcf.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gttxytdwp.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gxnzfaqtj.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gqhuyaqla.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gniocdbvv.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gzzyqcyfd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/ghblkprvg.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gohcxoiae.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/grmvcfdim.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gbgfvexmw.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gniiojxlm.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/guauopqsz.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/grbucfxap.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gnpuaacoe.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gdpwqzybg.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gsxtgnnuh.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gdpfuejww.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gkueylcpy.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gvblfnsdk.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gdmkkkvcj.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gidootjpm.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gqtzsidri.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/getqnxsep.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gohprusje.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gbqsqufrx.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gjpfhduzu.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gtzazfene.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gnhydeypo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gexnbiyhx.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gabxzuzqg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gybekdopz.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/goeanobps.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gomgcxtzh.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gysxdzpuo.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gewmdpaeb.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gxsdvdiom.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gxiqsjscm.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gssnqzswi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gnrsnyzyy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/ghonmekyi.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gbwzwvcms.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gztfmhgbw.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/garxsbgzr.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/ganfhmgte.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gakheprqn.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gnhaqwbor.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/guztrrsfs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gnlralpfr.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/guvifteyv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gbuzbmhni.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gfsyfihut.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/ggofqkesn.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gfiictmhg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gfcydaqmo.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gbmudtjcg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gnlftqmkk.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gqdswpfdh.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gfdhwarhw.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gbhklmiqm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gcrluhdfw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxxwndxpw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gbvspoysl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbwjzfprt.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gfswukdpy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gtoaiwylv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gjeaqcrbp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/grsvhoojc.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gblvnwcux.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gnhdpkrri.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gtdhuyfnq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gzqdudubq.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/garcbyxsc.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gldbzfkgq.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gdrunzsei.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gurpccwcr.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gaxrpyrun.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/guryolmzd.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gskhrzadb.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gjrxwadqb.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/glfwtcldb.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/golsnzrqf.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gbupxrfav.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gsjzslwsb.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gzfjvzzbb.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/grfkewbbq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gvvgaftwv.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/ggfldtjgw.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gvvuqovqw.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gcbxslmpk.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/glzuudqlc.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gltqucwmf.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gmjylhozv.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gtnsrvstf.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gqkduelqv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gvvklfnco.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gamaiqoxo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gkvxbpzbo.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gncajxmdt.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/ggeqbhtpt.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gzyqnlzxp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/giicjwzlh.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gqcdiwwlp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gampshyof.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gwkdtsrbf.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/grpjsfsts.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gtarleinm.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gmfluezkm.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gftawywmo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gwesrzfmj.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gzyiazbph.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gxkvnsxoo.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/ggebeiclw.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gazllmhjg.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gjtmimzic.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gszckvynb.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gckjohipk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gtsavqgwm.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gmsbjntfm.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/guedsmnvb.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gvtkpvofc.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gymcphyhp.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gypqfbilz.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/govabfuqr.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gwjktzrln.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/grawumpgg.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gurpkzmeh.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gqjhvxzib.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/garohyeoc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gqqirsrpc.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gbmecxzhw.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/ginmysriz.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gtpkpekqq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gntxvpchr.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gpdzpfqzn.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gvmfpsnpw.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gymusrual.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/ghezxfzza.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gxxfnxrwe.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/glgefjmfc.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gksvbutfs.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/geysmzjaa.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/ghyfpvqmo.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gscqzbkrw.sHtML


<!-- 参考信息 -->