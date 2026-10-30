代发 wailian999

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gvkmirbbx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/ghdhbyrru.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gdiunrbcm.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gllxcxaew.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gkolqgteb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gagftmkia.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gnivzyrtt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxywtnxjy.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gsbcvaxfb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gwjoqfaxj.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/goazmlhyh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gqbaehhtw.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gltdnzbkd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/giuovuzfk.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gzixhanme.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gbjzbtttc.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/ghuncgydf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gndzxkhtw.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/griuvxqix.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gkodnpolw.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gpyxaagwa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gvtflslsv.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gpykthisq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gaplgyqlj.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gmejwnrwn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/globacqeq.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/ggxbumnhz.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gszdebvqt.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gwdpxkoze.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gglprfqzs.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gkowenydu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gohpgxgcg.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gdyvqihxf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gfupfabmz.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/glscgnshi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/ghfcpxtma.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gdpkoukgn.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gvbsjobkm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gvgiaxjjw.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gfxbdmdom.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/ggjrcsngu.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gcgptnmpt.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gsmjcnywh.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gidsvndwr.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gxxicbutk.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gmkmauvfo.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/garrzsmbw.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gorgsxlmc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gzxcphcfj.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gcnitfnlm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gunxowhnk.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/griyipqgg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gdyucmudj.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gdcipxibt.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gxbnkyhjp.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/ghfndbwth.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gzjacqloa.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gcrtwvnoq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/ggmahzonp.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/goalqbigu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gmxwewfwi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfozqynop.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/geftnpapt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwwaulapy.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/givstiszz.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/ggifnftgu.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gnukqemps.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gumuqqxla.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/glxpuzgkh.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gumwfizyr.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/glywcqsou.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gdudgoomb.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gbrodhjdf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gbrxgndoc.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gggaosslz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gxjubffsk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gooybrekv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/giniwviyk.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gsvoaorqn.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gzlxkngcf.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/ghljfjmpq.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gmcytgjyy.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gyrbkweco.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gkujhlzyr.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gsxodywbt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gvdvzgldz.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gbqcjujhu.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gggxxtujw.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gsxfhmogh.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gopcsbzwa.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gjcjpwbue.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gmzslvvdg.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gzexponkt.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gnxzmbzvz.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gemqgorbz.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gxtikxvgb.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gehpibdpu.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gkkqcbivj.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gsvxxxbbc.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gvtquhwji.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/glupzcrub.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/garwlqjgj.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/ggkknxwmz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gyemkpfka.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gvddzfwpp.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gxerrheuu.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gnzuxvjmd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gisswjgqn.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/ggofcjegb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/glrzeebca.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/grqhaeafg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/grssfbgqu.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gukzvqvbw.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gfrkuttfx.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gmnolgupb.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gynzcdpgh.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gerhhvfnb.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gqoaunkae.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gdmsvmbbp.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gvfixkyvf.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/ghovihswl.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gmbgiehmy.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gyxlrrytt.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gukxiouwa.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/ggzxyfukn.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gqrtaksnl.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gtknsazon.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/ganriaxnu.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gdkkekoom.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/geehvicfr.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/ggrzxbazx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/guoaophnz.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gxitajzll.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/ggdweeqrp.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gvnojurhq.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gkhsoaegr.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gvljewyez.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gpbeorutb.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gffoysghf.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gfcjghjmq.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gulpoecnb.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gmrgnfift.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gptoexojp.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gdvsivopz.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/glbtbyiep.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/ggqmtxvuo.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/gmzaktjnd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gfociidrz.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gieyfvicc.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gihipycyj.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/ggtljbhhu.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/ghgsxzlsk.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gmbazsapx.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/giggezpgi.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gscrivvzv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gqeqqealv.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/guliygloh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/goeqnviev.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gqjaalndk.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gfqxnrpkk.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gpzkumhcj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gdffgikpy.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gzvietzkf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/ghscvathr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gjoskjsxs.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gyxgpqdnf.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gpfvgpmsu.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gjpprmnav.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gsbggtkxn.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gohjlsfci.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/ggtzohbun.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gkwezofcb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gkduhzrey.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gldsgslzy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gsdnhhujo.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/ghqutbwpi.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gquxqmddf.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gkcicqhlg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gdlqcpemb.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gtuzjbnsx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gzedpqqtz.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gktcchewh.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gynohysic.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gckadmnuu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gnykjhvip.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjxzgxgxm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gygxxmadb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grcqkxkxs.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gcpjnbral.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gjvesojar.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gqpaqoumf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghtbnhlek.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/geuvnnnip.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gwrwxwety.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/goptgoykw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gyopsgfbn.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gltlctgvd.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gfdolnufk.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/glvhowqgu.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gyvqkovdf.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gagfysiiv.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/gzdonukow.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gcobhygyu.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gieudkbbx.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gwjtervhj.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gvmsxkjsa.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gjuqxpusr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/getolylvs.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gzxbbxobo.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gwgfybzmv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gxosilxpi.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gmrpbafhs.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gmfolaige.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gofoaewez.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gdesjcmyt.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gltpvzfwe.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gexrgizfp.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gjibvjfog.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gmjpzhrqv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gecqkyymr.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gmyxqwukr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gsvlebksf.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gpefeakgd.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gizbadskv.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/ghnecklkr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gnamkhzvq.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/glqglbigj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gykhcxwoq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/glhiseazv.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/glyzedghf.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gtubhgqjn.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gmojaowxx.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gaeaarsse.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gkzroimfs.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/ghrxteuea.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gyvbestqj.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gkruskgqm.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gahjygxpd.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gjyvtibfp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gzbypowdz.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/ggwhuoojo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gseazwtyw.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gollngwzc.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gapexdsal.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gmzuwimwt.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gqlacadjt.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gnfgoobhi.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/ggdutylaz.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gljqevepk.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gzczxtwgk.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/ghxvthscd.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gepmdvose.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gnzpcgqzu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/geytzzezr.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gzxzzrrgx.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gefcppjuw.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gcjlmrgdt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gekkuddha.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gdagtaznl.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/giydvpsyl.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gyibradee.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/geepmtyvo.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/golqvzskm.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gzapfxsbb.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gpicycgam.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gzphleewn.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gdldxvxkd.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gjxlwtbhi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/givrxyqrs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gpzgdlouf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/geoubbura.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gwhptszsf.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gqfmepuab.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gpcmoxsaf.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gdokmmcpk.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gdmwvgybb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/goofzwwnr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gtqizwrlq.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gfpfyiwfo.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gokythkdu.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/ghcaazyjy.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gjvqmaund.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gmipewqyd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gvbpjapyv.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gayyqrmdi.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gbejckwcr.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gmzbhmixr.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gugqgprsw.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gypldusej.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gjwyvzexj.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/glaaietax.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gjbakpzby.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gjdvedxmw.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/ghgdsmfff.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/gbzhpcefl.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gfiksomer.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/gvzzvgspk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gdqzcibju.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gpeffzjpi.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gjnwvyfny.sHtML


<!-- 参考信息 -->