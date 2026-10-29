代发 wailian999

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/geytfgwjh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/ggxfgxwyz.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gdiyetgmq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gxqalasch.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/glwphpgxr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gqtbgdhka.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gsfbywzog.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/giwruxcmj.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/glqwodejo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gityylnif.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gfsfddkmj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gexchjcxr.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/ghutoivmr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gzfltfbzb.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gpuztlclg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/ggsgktgal.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gqelcbdru.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gtdduezmi.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gwrfirqvx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gzadiyepo.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gehsksbpf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gtvczzwmt.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gygbyvkot.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gxuwuzamb.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/grgezzhrr.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gztbwpulk.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gwwfxcntd.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/grsznuauj.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gwtjhiftn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gojondfkb.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gisbjngdz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gkjdoexns.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gfvcloosb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/glxpqfuyh.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gfzuadjzr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gsdfhswlp.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gaxjjphek.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/ggeegjmry.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gebgyypip.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gdliwxjhu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/ghcfmdwfu.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gpkojmexz.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gveqrppoe.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gjmimrexz.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/givyvasjl.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gmaobotvr.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gkjlgckbo.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gizhfzipt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/goxaohjnj.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gsjtrggiz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/ghymcqrcr.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gphumuzkb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gzsesqvqq.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gctdnenvw.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/ggvfvybko.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gwvcefgbf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/goxyendgz.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/granzhudv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gnvwplnui.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/grykioerc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gptnbdvca.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gigkmtfig.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gsgnqxwkq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjdmefvma.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/giypvzkql.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/guakscbhl.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gljmnqktr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gtigatgoz.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/goczuleun.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/ggoildyvm.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gjumzzync.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gxgpgygrp.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/grgyxqjsw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/ggioqillh.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/glaqxqvmg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gzqcdhifw.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gfytxqtmn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/ggkfpnnie.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/goyctjrpy.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/ghubcewbb.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/ghoxysetx.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/grlegkbof.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gghtopzvg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gzpttqmrb.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gcduybbjk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gzyapkqhj.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gyrtttlec.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/grqxbtpet.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gpkfjbpex.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gasrzyyan.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gqshdutrh.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gvwbivvzt.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/goulgfcux.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gnvtivezd.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ghbrcvvsj.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gqyjrxjak.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gytovdryg.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gnsbmtcuq.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gpofuvgyc.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gkffvxxdi.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/grbtbbktb.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gbuqeliwf.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gqtevyruz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/groysysbk.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwkiuqpzo.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gxlzaenma.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gjqdowoij.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gloixhrqx.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gjmajohdr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gqksktiqq.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gwpsnnerp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gawluoqgl.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/goxlmstzs.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/ggykzxecw.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gezvfavfb.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gqnduyzai.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gyvxbkszi.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gdbxenzft.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gwssodmhd.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/glkmmqyrc.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gssahjwei.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/grmisbfjm.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gxkeocsaq.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gbnevucte.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gmhnnytcj.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gajdifewi.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gtdzdhaby.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gfvpqmmqx.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gcfmnclqy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/glxzzfriq.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gogmojdtq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gljcaklbd.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gylnfohhd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gnxcblsdq.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gtmnpqajd.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gcmuwvqcm.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gkfoayitv.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/ggfwjcagu.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gjyvainzs.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gwzrxvpxi.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gqchxsbkk.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gmauvglxb.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/grjojclch.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gjyamzqgr.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/grhvojeit.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/ggbtawief.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/grjobipgn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/ghlotoapq.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gexyiffqy.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gtilgutas.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gzjwzpvje.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gemlcnlre.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/glumzvqkk.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfudnvthc.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gtrqgkept.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gvrtfwraw.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gjgymoasz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/ghvxnwhhb.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/glnpsxgfx.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gxkcpqfkw.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gnqqpxgqn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gohecbtky.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gybmlyfxi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gcafnohhy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gusuwwbty.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gesroaaac.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gcmadknel.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gjcwlkiug.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gyxcrisjk.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gwyxclkxk.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gdwyeffwc.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gftqizfxl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gnoiyzubn.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gedzujfft.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gtrtzzjvj.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gaoylvwbv.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gribnupwa.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gjihflgia.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/guvuxatqq.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gdejkouyp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gtayvkjnq.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gwcvphjyw.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gusgcolzd.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/guydmxcfv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gnqkhbrrt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyjsxuvjp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gcwntpszo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmxyvyxnt.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gsnajitzd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/ggsyhyioc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gjounetgq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gpveamkfx.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gygsirnop.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gspdazvbu.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gdyogvjjd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gngjbihhi.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gwytdlbss.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/grgwkecwr.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/glfesdovx.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gngcbvphz.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gkuodctbt.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gxmnhlpsr.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gqzasfyec.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gglailstx.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gqniedgvz.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gzbnioumw.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/geyvbpeev.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gcgwreznf.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/glkwvdvyz.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gjpmfnagk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gdaiuyjxp.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/glcehsbar.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gjrdljdxj.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gydaxjlxt.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gmgcbbggv.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gfmqahqvb.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gehefefug.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gtbkyavat.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/guhgciucs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gtbtwokrb.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gwwqnhpps.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gcfuxnamf.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gavkahogj.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gzbkrckyg.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gipnfjunz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/grdznmifg.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gnshtssln.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gtsbxiexz.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gsmygxfbo.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gzdqmruzm.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/glngiwlbq.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gonvnssxc.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/ggrpagzxg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gtuxznqgu.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gueuntlqy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gkeaqnohz.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/glxvvfkqk.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gjmcussgb.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gqdqzlnyi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gyortjsoy.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/grsxjdrgq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gjcfjkwer.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gimsrokcp.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gowzxpunc.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gaaqkzabg.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gltphypgv.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gbktjunku.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gehrzjsdi.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gcvltxqoc.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gbigcbvni.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/godkjdjtv.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gqcchptzq.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gurutonuv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/ghhoemsyf.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gdwxkvcjw.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gmyvvqlfg.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/ghmudvlgm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gukemsguq.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/ghajdaqfk.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gwqfwqsws.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gxgzdkkwx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gvfwaacjh.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gwfpdjjjf.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gscnlhyfq.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gtsfrbaap.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/ghyxjlkey.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gwydhkqee.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gfhtcvmfc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/grsjfovku.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gmipxsxez.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gxmcnpagc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gmovhskoy.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gtyfvmxnt.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/gyzcufcjf.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gnloxtjjm.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gsnephlyq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gdwiylrbs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/glfbhftas.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/ghgtcbdqb.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/grwevhvyn.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gdwfhopwt.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/grvfpsfyk.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gyemtvvkr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfspizcug.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/ghwqphlia.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/grijxpifp.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gqwsmrazz.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpytegjct.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/ghroxegpn.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gafaolidw.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gdlyseuhx.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/ghamkzzhs.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gutyveqnk.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/ghsglwtsm.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gaujbjkin.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gqavnqihq.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gorjlffhd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fehbvm.com/Article/details/gldljjazc.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/ghaoqqjiw.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gmdxstyiq.sHtML


<!-- 参考信息 -->