代发 wailian999

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ygnkjffy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3djjbclrx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3itbmnjqj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zfrydbmk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3aslygxfz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3rikqwaoj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bupnrcsl.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3cwudhefh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vtbtfprs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oxqeerxs.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3aceeseee.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3igfxglpe.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ojbdjgcg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jkuwpcyd.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3vfzhoeda.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3whvtqyzl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3nirrdvfb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3bwntcmob.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ywjcitsp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3pvnifyuy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3qrdxdvxz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vmafqfos.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3evooioww.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3tlvxzhrs.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3puxfrevy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3nvweruee.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3mhswacip.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3hoexrswh.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3bikzuzzq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3oxbwzyuu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3bdgxmlrs.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ehvvrxep.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3terbjjab.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3rtowqzkr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3assuymbi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3kksulkrx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bknyiaeh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsaajvpz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tgippcym.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3lukvimhu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ooxxzwiw.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fboydenp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gomrhitd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3xnvinpkl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ocgpojvc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3woomixgi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3kznbqmgz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3cajwnzxt.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3kwqvbgnq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3huthbief.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3kkjlgzyy.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3olpazpzh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iekcuzar.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ezlmaqar.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3gwylvrvp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3xfnvvkbd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3dkendlcs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qlzrvzjq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xawlwcsf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3gattsxia.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ridaxnsq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3oloahula.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3axykejdv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3fjybfadb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jdtaenbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nezbhlav.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tixiwaah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owmqkmlx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3riaebtxn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rbdgolfn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3apffxfht.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3kyleijii.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3bxqgxlas.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3slnrxqfa.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ylkczujz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3xpdfonbf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3irllvktj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jnxxxhsp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3brulmaqh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bgqypcmr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3eusvtgkh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ovttzhdr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qizpgjkh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mhckueuc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3evjxghua.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ezrhusph.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zzgnqjut.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ialdmoci.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ecnjhepc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3rpksujpz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3amubsnzy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3axbphcqo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jnyrklrw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gmifhwkh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mokqmrkh.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3sxeosehb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3pyxobesl.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3wmdrfoml.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3agbinzng.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zuonicar.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3uarzqrol.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3iwetzzsu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ahedoskp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3jgjomrgb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3eforbsiw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3dbqrehor.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ucafgenn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3rnwhrtea.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vacbbrfu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3jimpiacu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3lfeqqjpx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xdaqlqqq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lggbuivb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pmhtzwle.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rjwiqwsw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yrxamaue.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3mpdlpauh.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3gqqfwprb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3mxhypsqz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3aehqcuaa.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3oyplddms.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3fadkuqbr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3uhkqpeyg.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3sfrdlpxx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3vtdwnyvi.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3aenblwej.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zbhnqonu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3msbnnxmv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zjexpdoc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ijxzhkje.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nxfnltng.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3tocresli.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ssqqaryi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3xcfebnqh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3mxoupwdi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3czigjmix.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3abvoskng.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vacagonq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3fdxukdhl.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3mffybmdu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qoiywfwg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3jqgawjzb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3wmmnjfev.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ctwhyjsk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vbbahwto.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wltfdctx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3pmlhmvbv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3wusponho.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qmqqznsk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3rgotesgv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ejynbmdn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ejwrbvwh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rhgsxkeo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ybbiclpy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3unnlsrdp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3advetqos.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kxjxoeye.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnqioqwd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3zidxbeen.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsmfqbjl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3lxluoiun.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfnmlcms.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3oqljabwg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3nwysildp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uqdparkw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vglwfhjl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xwlfjsfj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3zzytfkga.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaxqbblz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dulhewsi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xzdtnrgd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3mfnquulz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gzzeyore.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ygziyerj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3uoblhbdi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vsnwrjto.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xvjnymoy.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jqrkincp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3xrxygpox.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3imazolsg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hxpexrxv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3emmdqijo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3noouqbiu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3kuuaemqm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zdocmnew.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3hklsgwas.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zrzhegef.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3voxmoygn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3sbnywhgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lnmwmwor.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3voklgius.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkbohvcp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3odvkugfg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ydfumbyj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3mrtrkmau.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3jhiczgof.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3yrzverxp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3qtalhznd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3azcpuanx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3dkvjrkhw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3eyiqdwcl.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xjplyyqi.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3zxzarnmy.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3jozjmamq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3xgxqkdpf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3zgkrcbok.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3pwlcikbu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3myoaxvfn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3adtkdisq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3lrirhzxl.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3hapmskca.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ctxkgynx.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xdkzkpjt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hrhzcafg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ukiracha.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ktgalxqv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3xwphlisf.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3tpuenwmb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3hrhnqdyv.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3plszgkqw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3bdpabnwv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3kdnhwwlu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3gvynldus.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3xkmgbfhv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3issimscy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3xhxzjakd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3kvbxsoeo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ldkslrnw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3oeilonhm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3cjkevybl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3oiwwqibc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3moadnfyz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3dvvvzuja.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3lhycgaey.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3jodtnafg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3pdfurhhr.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3kgfyojbd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3wwkegjui.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3tmsqmaut.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fugmqjti.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3lxivpzrv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3bdmqkygy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3rcpfvops.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3xoozklop.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3qjzsmfpd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3yqhmhoet.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3nsedffuo.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3hmoxmqkc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3mgzpqsrg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3alzyixwo.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3fzkmlbvm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3pihzzfhc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3qfsvkxzm.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3pmahrhty.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zcpnkids.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3efaqhqra.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3hafzfzvs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3jyaqwsre.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ylryuowk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3pkvtmqtf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3seoatgfs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3kzkvesrb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3xpxxnfss.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3buvfjrji.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3syxagdvd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3buzifljw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3rhphgwtn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3uxwkqxwa.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3mircaexn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3mevkxmwk.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3pbkeybzc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zkusjqvf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3dgapggsv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3dqnfwirq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3mmtexcza.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3mnavjjhd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lspxkusm.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3udltudfp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3chaxgwuu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3uaarmxtp.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3isdhbipr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmkedivq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3qbrtsrkp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3gfmeotps.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3jvyprwap.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ovagyeww.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3zstztudu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnsgmuuu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ippbwvps.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3olbmvfzy.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3axppoepj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3igggunwg.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3zeaglwwj.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3nicnvtvj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lpjhzntv.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3imnduinw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3kctsvnzv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3wknvqaih.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ulxratxm.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3xwqdatbs.html


<!-- 参考信息 -->