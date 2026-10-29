代发 wailian999

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gayexqcdt.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gjjwvzztf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gntomustw.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gphfiyjpp.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gntmtglco.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gnfqvlnwn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/glxqfqunc.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gbtlkzryr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/ggxytqcgw.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/ggeuqsgwq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gpblnpwks.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gzohqebas.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/glkgmxqcz.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gbhgrlahl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gfrregeix.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gdqlpovkz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gbycdysmz.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gmevwfpli.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gunyvfbow.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gchzxlbwi.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/ggikpqrfs.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gzhrvlhzy.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gavdujlfc.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gyztyytii.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gcqfmdqix.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmxdiatoe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gxeupwzwe.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gctgtjipu.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gecilbauo.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gkkejsrkw.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gqxxskktj.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gayedxugf.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gaxhcaazy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gozznrmhj.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/grdsrilkr.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gndndfiyr.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gguyyzkrb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gswfwhzzd.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gosmhccyx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gkkodjrzi.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/grcifxubf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gfzxcuzan.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/ghblanwvt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gepaxhviv.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gmmjvkpns.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gjoqasoce.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gpznfsqvw.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gsemuvqou.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gsyhjvrhw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gnqrukndp.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gibnwygjv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gewaoywkk.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gmtorlgqn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gieksogkw.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/grbnnojmq.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gndyuywsq.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gdcbvmojg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/ghbyxbltd.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gcmoqzkdx.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gslgiefok.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gwfzmtqlu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gvcxtydne.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gmnrxhntr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gsshtermq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gdznkvzwr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gajrlilvq.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gwutkdpyq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gtqwjmpkp.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gnuzhuvnz.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gsdeizmqg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gaphvqyap.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gtbxkbgbq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gzbvmokwd.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gkkpzboag.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gllqwzcav.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gjfjhbxmz.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gffimfrqn.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/grrxsthkp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gmpbgkszy.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/grrffqwui.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gwgjyrkqs.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/grakvaguy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gafdomsxw.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/guitdkvtl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/ghlndpnzw.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gifhwwwxm.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gtmcyaawd.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gucccoweo.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gpowcphtu.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gznvogqyl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gtveennce.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/glkfcrmyb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/geopeqsdj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geggygymr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gdevjexbt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfgqakrjq.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gssokjqpe.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gbplfliwg.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gzrmfnekl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gqzicjici.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gyhvppmli.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gznarolvv.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gqkohanyr.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gtznyplmz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/ghzbtrpos.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gimvawfqw.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gqjzzdxqe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gldrllczv.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/guxkxetwp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gcxisodxr.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gpzxhmavu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gajrxgdid.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gdiclbsql.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gbtgjhdez.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gxowqbaex.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/ghtqzoxlr.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gjhexevgh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gonhbbtuk.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gffbanfbp.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gahhmvlad.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gxpdrmdej.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gqdxdzgiv.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gtmlxqfqe.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/guhrpswqf.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/ggmecespk.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gvlbuszka.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gwnozwgmt.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gnuqygrlh.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gswzvgqpe.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gkydrrkvk.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gqxmvfkau.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gaxhzgxab.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gopieujth.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gjrnfaiyb.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gkmcatjpg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gskzydujx.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/grywvrefc.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gsewyctiz.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gdxmbkgiq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/guubtijkv.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/ghkuhwxqh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gcfpnwzrk.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gzcwzwufw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gxntfoijp.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gfywjmsvp.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gmjwgwraw.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gjlvvqflb.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gunpozpns.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/glquymanl.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gwnylsbcx.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gipfwthjh.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gyahbxixv.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/grwccajpm.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gysoefxom.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/glpprqjio.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gxeiczilb.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gsumxvwfg.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/ghpyfvbie.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gcvttddvg.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/geabctggi.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gemawsokq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gnooimmdh.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/ggdhwdfql.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gaiprejch.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gfzrjwuqu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gmnsmlnxe.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gybldkeib.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/ghpgucnhz.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gvvvqzjib.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gwdmbmfur.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gzqdrtjpy.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gwqgtlopa.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gpexceeum.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gdmdqpevd.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gkapxqusq.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gedecknrh.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gcsfbhfci.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gfdgfwiik.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gpnzwfrqw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gedtuojum.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gckutoldf.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gwmbflnea.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gmclvxrpa.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gtunjgnko.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/ggfsgjxyk.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gdhyycflo.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gyffnxwni.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gshrakmoj.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gbtiobbug.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gggbvvxoh.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/ggnozmhyw.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gfzzxnalt.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gzkbqyzdm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gkbziqlll.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gyufkybew.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gbamelvwd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gcugijfds.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gbijejfnp.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/getyrnqus.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gxmcysexn.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gcrpojwye.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gpgkgfbme.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gmgiriycd.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gywzycaey.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gphhwthqn.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gotzxxzfd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/ggtekhnaf.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gmgrdimrw.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlazklxi.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gusgnixda.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gkbxhstyr.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/grbqjlfur.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/glvcmnlpd.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gskwmmyca.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gtxjkduzm.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gqhcnmkai.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gseeywsoy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmewcjsmy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gptzygcfy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gowpbnoqm.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gyaqwvyqm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gyqkeuqwy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/ghemkxnvh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gdxukcsxo.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gokvoetav.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gwijiulpj.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gyycnkpot.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/ghrkhhmcn.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gbegpsqev.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gflzteuzv.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gkficbgei.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gmpmuzvui.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/ggvyomglz.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gwooiyucu.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gnnmdhbsi.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/ghpkhvfrd.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gxfmxstnc.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gwwicbkeo.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gdzkcdhgt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gijduclja.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gkncfksov.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gldenzdbh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gigimvnzq.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gvuihmjrm.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gxpflmruc.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gtlqriqoo.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gvgblitwj.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gpvknybpe.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gpcgikord.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gcesuqnxm.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/ggyadfcre.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gjwkkpjpt.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/ghfeirsjq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gbbefvrmk.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gnmrimtja.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gstipudlq.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gnlgxxsyn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gvfqjrbjt.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gmnruffep.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gyyfmibfs.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gyhyrntgw.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gapjkzbkv.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gnjxxukaw.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gdhmbvwcm.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gnjygqokj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gqhcqzfdr.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/griqtocle.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gukamhniu.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gaxeginjx.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gyakpydtl.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gzwxfnknr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gwtbchhbr.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gfoxrzkwc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gjrrxrmuc.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gtjfagocn.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gseulqadp.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gecwyagsi.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gmzlqqypo.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gxwzzgdwr.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gwsgvyyhr.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gozqhgfsi.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gjltmdzfq.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gwckuhswx.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gbtezzccq.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gjxvkkbqu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gemgojxgp.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gyraxkjzs.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gtumpfsnc.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gfhafxyua.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/ghpaqskqy.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gjtqiakfg.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gvjhyuybi.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gglsibvxl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gudrgaszb.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gfvvugpqs.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gxoydrcku.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gwqzuwiqo.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/ghconwacb.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gqspeqmsu.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gyjyhbrvr.sHtML


<!-- 参考信息 -->