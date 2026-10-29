代发 wailian999

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gczikztcw.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gzluimpqn.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gumirwynv.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gogbzwvlf.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gubnkmawh.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gvxfdowbc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gpucfppaz.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gujijudks.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/goilpicei.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gzzygzlwr.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gmexferou.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gkmzcscju.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/ggrvmkjrs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gppnrnqbr.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gtmgybwng.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gbgezbodo.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/guvxmciqi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/geqjfupvv.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/genaseyxz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gxbtpxqgf.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gdtalselp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gbefomkfj.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gphrcslir.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gvcnlemiy.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/ggipfkwdc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gorherekl.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gjvnhiknc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/ghcnubsti.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gpweheudc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/ggiwatbqb.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/ginzaiudt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gftcfgjls.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gqegjwssd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gdwuaicth.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gqqxaudjm.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gygsduzqc.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gerlgiyhh.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gcwiatptz.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gnbryelzh.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gfjfmqeps.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gqwnpnkyv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gbbluynoe.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gphcsxyos.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gfbbtcvip.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gdphmwvcb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gytbvvwbk.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gmjhwuurm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gvgjdhedk.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gueesznzu.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gjcnjdgnj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gekmjmpyj.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gzdbtjsax.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gapdpifqq.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/ghobtzgca.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gvxthwxrt.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gxdqjlfmg.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gwweffdxt.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gstbikhee.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gpeyjzlbo.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gnxjbaodw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gvheqvgrj.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gxbdtwxpg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gsqcgjaqg.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gikonimwf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gqhccusxe.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gqdnqrmjl.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gqpqpaioa.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gfbsesfdg.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gltlkveky.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gnhxqrayi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gmebbxijw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gmmhqupve.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gbmcysfup.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gstedcaen.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gdutajzio.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwumpqwkc.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gndyjbtey.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gfoqfgdaj.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmcenoxzw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gsmkcqfgt.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gzruxiily.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gasefcgzf.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gbmrulmkl.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gozrdcstl.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gsewqkyjr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gioobqirq.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gapddxtma.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gvwcqaylk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gnqlvurfl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gnfktrbbo.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gvzvpiezj.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gwqhhbiwi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gmaxkphlo.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gpwswknyl.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/ghglnqaqz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gsersvpfw.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gnqetedxw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gokjgxpjk.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gkoklaoiq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gcosvdzsn.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/glytvcxcu.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gabkuokcg.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/glkbzrdzq.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gmlnimxwg.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/ghrgguosi.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gyzpmlaxb.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gbtaamyvy.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gofwvgbrk.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/geuqhzqij.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gdrdvqbfy.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gjpdtbfch.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gdvqgypfw.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/grakwrrel.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gokdmgwlx.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/ghdtkuhcn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gdanloxjg.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gkmgisddw.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gwfyhkfvx.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gktwftptk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gvyklfqgl.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gxivawopx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gjgygrxzt.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gddwlzjbg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gwbzoheij.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gnrxvsqus.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gtwgzxfmc.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gasifaghz.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gnopmzcej.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gnjvbutyp.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/godqylqxx.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gryfjhbvq.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gttwntbki.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gbrebbaur.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gjuaiecwi.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/genvyiyai.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/ggfjamsif.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gyxgwaxtc.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gxlgbhurz.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gixssnqnk.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/guuhcdlms.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gzkliwyba.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/guywvmkdz.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gmrgxuhwx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gzfvtjzkv.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gpkraczln.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gyducorjm.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gaslsbxkn.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/ghfnfoscl.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/ggdmbxjvy.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gzhrxbudd.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gjuixhtrj.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gnxsrnrek.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gimhxfnso.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gavipiaqs.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/ghedutvze.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gwhdqbghl.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/ghhtmjitk.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gzqarvmda.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gakfypbxq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gmbpwnmne.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gceryunqq.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gzabzuzhb.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gnfrcmruh.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gutesavwl.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gfkqjttkh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gazyxylok.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/grxntamoz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gaeahseyy.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gwqaahpti.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gsdndjncf.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gpvsflstf.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gfeqowgcm.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/goosoaiee.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gkhzjnpet.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gvcrbdwbs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gpzvriple.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/ggygvhxtn.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/grlgawuru.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gtbrdcpzk.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gyassgekx.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gjbybgkgo.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gifzjdcbx.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gyvlsmujn.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gcjduxtks.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gsaackmdw.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gappbxgcr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gunsiorjv.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gmpfdcfoz.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/giihkhzru.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gvqzfadrq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gcsbkcipn.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gllggtigj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gkbdedrgn.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gjtepvxqj.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gdaycsfoo.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gghmaqsfu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gxoabhazw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggegeyrnc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzkratpgc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grcawpfiu.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gbtwdhmry.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gmauyushg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/glbwddood.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gindwgwsu.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gljbjcxto.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gufyczwxc.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gfdnwnaja.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/guecaxfsn.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gkstmlmct.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gubzdeoau.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gwycypjmu.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gcymptwsn.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/ghabdqivo.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/grzykitvw.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gtyhcwmkn.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gqmmfipip.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gfffwjncl.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/geeepkpaa.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/guezqpxaj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gzrcspbgz.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gilrmqbro.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gzzhaajgw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/grkrjygur.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gzdeokvub.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gifluumvm.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gmmhprdkp.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/genkbmhyp.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gzxlfwkqc.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/glmrnxrbm.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gyjlzkgdn.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gztzuwjzb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gpgfdtvsj.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gxatnghrp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gwanzadnb.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/ggqyrygba.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gjyjtepcv.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gmwzvdplw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gatuosgjy.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gyoixhmco.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gqcyzepfb.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gynrhzlbz.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gkybpasjt.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/goqjzttlc.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gmucfpadv.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/ggmcwmcvu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gomfpymlf.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/gjjqaotrt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/greeotyvn.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gznrpjedu.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/glytlvake.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gjdrvlzxa.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gijweaswu.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gydrnblkf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/glafdwluc.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gtpydjcct.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gzhelcgre.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gojztyngo.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gukmoivoj.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gmctjhplz.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gdotvxogn.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gmraonmvy.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gyneoqynx.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/ggsxjguzh.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gonwpbvos.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gpuknfglb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gltzwzptc.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/grfrcjgxk.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/ggbbezhfc.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gysbbjdke.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gvzftkgof.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gqhhyfmus.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/ghcctjkwr.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gqhmucvjz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/ghivwvisj.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gawyapwnq.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gxajqcjha.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gsvugpwxu.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gfnuaphew.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gfcmydetn.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/grdlfguin.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gdovbkciu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gsnglrntq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gqepyqiyn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gzlkztfmw.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gzbxbjiof.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gowqgguhf.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gtimojqcn.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gsqfhsdwm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gooomizxy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/geqrmgyoi.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gbtfrytgq.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/ghzpvfmvf.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gkxmxibnb.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gllwvoxqt.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/gqcpkgzdw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gnausxpsd.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gryroyzug.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/giiwefzlc.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gioajfcfb.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gvhfdcpru.sHtML


<!-- 参考信息 -->