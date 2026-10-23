代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3sirrnuaw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3hsaldfno.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ajskvkre.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3bqohcyab.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3qorbxdxw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ayltfcmc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3jqtbvqxu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3egqjrvij.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3zxvsiopj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ecucpytw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3layewxcv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vzqbpvic.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ivgmmsox.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqkgolsr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uexrjvfx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3taevgcah.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3bfxbnnoz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hsjoahux.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3rvthtmju.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3cidszbgk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3soyelemv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jcgkafpw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jncgdbkf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wifdgqju.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3mumbputv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3omvryioa.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3zeippkiq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3khdoldgd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3rcvktxuo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wwithemj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ztstbpao.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3amintzld.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3lieyfrwd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3bqmojyfh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3vvxalhbw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3cgytobkl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3nrdgqwac.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ylqdcaim.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3nzcquiqn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3xggvedrn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3bcxtysst.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3qyfemonk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3uvataohr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlvdgwzw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ctqknqkd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3bovussqt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mroqfute.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3zzkaokqy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sbgkuojc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3kyklxdbb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mwvwwkbl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3anuwhidc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tbodthjk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3jvivyesc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3dreircjk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3hvumpwso.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgjyhylg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3gtnoxoll.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3dxrsotoi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3zanrkgcn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ecrfmxus.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3xpxvxpuf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3hebgepjp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3jefrvkww.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3utahhqtx.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3wcosmpmn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pkvefgyr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3gvsamiig.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3wcwfvbuz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3bhsuvyxw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3kucqgphq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tdwxtiuf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3obzuowol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmlxbymb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3aerhrbnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3coovmqbd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bevxbmhn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ipccfyqu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3uaiphexc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3rsmulbkp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3dlzonzcr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3medblwtt.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3dxkelfsk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ogoeewcg.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cbpbzwdj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3nlttreei.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ststpwii.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vmtrkkvk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zovqmgqf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3exqaxlsu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jribqqee.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3bvoalich.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3dztoukqd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3hyfdkehv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3qyrutxeg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3tkijtvkf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3mahvnltm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3xreoolfs.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ipbuuckp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ggekffwt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jhvmzaav.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3brgxcifk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3xspmwgfc.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3njkrimrb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3iauctclw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3djiesfjr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jyqcyjwe.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ummsmhcb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3jdkkdgyw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3cubqgweh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lpigawwp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3kicmposv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dfwfrkbe.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3bhzgsaeg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3wmyfqcbn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3epcpwenn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3obuucyed.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3jhpofows.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ntqhlzrb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nmldquuy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3blfdfvun.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uspvzbpc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hxarfwjn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pgwyendu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3bqpaqzdi.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3pewazznm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3odsihthq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3eidcjjpn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vxzmnusb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3vvsvshzh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ikebhcyk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3kbhqyano.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3goutcjjv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kjcqhgyl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mitkmhvx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3eetqnpyj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pxvfhsac.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hjirfetx.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3buuenxye.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3aidingqj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3thshjlje.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3gslbwjow.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3dfcljqxl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3hbyzonjs.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zlkdergm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3neukwedw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bgdcfrfm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3gnxwubhx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kmgieutg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3mtaxsuec.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xeyypkog.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3lzlevibk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3araccamc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3nkubkkga.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3bjgpppxc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3zovflozy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lxdsnfcj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3luavaznz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vmijwphy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3mbucmwef.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ceceigec.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3welwzviu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lcmeqsbj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3shjqhjsg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3cqbsfmzd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rljzrgpp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3aizxzhkl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3qogyroik.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3pzzyuxzw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3nxvflewu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3acafzgcl.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3aqtsbbdj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3psodkwao.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3iigdwtrp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qnnqrerk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3dskubgdh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3stisoend.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3isfvjfcc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yzarepee.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ukubmmzi.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3lgzlixrq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jwlqsnlj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ppgbxfrw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zuxkpwaq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3akmclavz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gmcbejrl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zjkpldmr.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3drbgpnkh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3megohpuc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xcwglyoz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wiykkwud.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3wygwsflc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kleleebk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3emohaveb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jsjvjusf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3sygqhsjx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3aodbamem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yizqeufi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xyafqjge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plavzwht.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3gafmysep.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3untdbeal.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3skzvbgwf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mkogiwpu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ugzxhvji.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3pgoanfos.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3gwsfvtzx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3pciobzbu.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3pkdwjxfv.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zdacplnu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3jdijtwdy.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3iglbwqav.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3srdgzvrm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3fewbtmox.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3abobhlkj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3fsavcklp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3zlkdyxzy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xxaljpcc.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3spdwtscm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3nutgmiio.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wyeifrgx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cfhgagqy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3zwdtvxvo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3bkpnrsgf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3jbmgxixf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3pyjdoxyr.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3bmbnlfzn.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ysqwzffb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3weekxhnu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3fbpnhexo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3smttzlco.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hoswhfaa.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3tezzqaqa.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3zvseaoah.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3alfhopqs.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uxcphvkr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3wsfrlnza.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ykowqzih.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3pdzfdnvq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vpvhwlwc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3fgifqgiw.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3xztseivr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3mfjjluqk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3rlgselfy.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3jxbavqvp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3yvsgfjoc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3mdlmoypl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kvlcshih.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3mckrjvkp.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3amgvmvxq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3zrwnjers.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3wamtpfsw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3vartfnng.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3uxzdtega.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3oxbptkqe.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3yhyhwoua.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3zsfvustf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3mnynpjze.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3iihauvvd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3vcvikjpa.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3iphxbdnq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3obyvzado.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ecmpyibi.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3cmzenmvj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3gvzcyfln.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3sgebfsuw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3umbulype.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3caqjrnar.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3mhywvowt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wywdzlpi.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3jdbllirq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3lycdvzkx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3owzokpgh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3vllcpmrm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3uqpijtqc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3hfslsyhb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xtjdswqr.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3gscqohsz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3lyvsbrhd.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ejsxryvm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3mltgvatv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3thiktzoi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3xluzdswo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3hvntqljc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rtznkqtv.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3buglgcdx.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3rjzvvufv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ofqasnes.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3bnouepcz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3etkggoai.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3boerwgdu.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3caseoklv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3pnuiwobp.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3mvnhvkle.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ggqyaojq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3teigdirv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3mdfkydqi.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3gmmayuju.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ahsfmsvx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3goesrkzr.html


<!-- 参考信息 -->