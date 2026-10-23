代发 wailian999

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3szzfhopo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3lflpqrsb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3arrkfzst.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3sabedhqo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3tqmwnagx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dmesmbjg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hmzdvixw.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tvwntgpj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3eitubmxs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndmesjsb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3khrsogkv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3amxixdng.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3dnluwbpy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3inkkfped.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3hessczxk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3fpjrpwjr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ajnuunuc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xygkgant.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3wngngcbl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ijaiugaj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3luwiirnf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wmyqwyvw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ghlyhnpa.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3esajggiv.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3llrntwcg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3nkszjhsz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3zdsibqsy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3njlthabf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ytvnzosp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ghtuwjxd.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3csqcqsym.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3gansbuik.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3nysxoogh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mlwobpja.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ggcgcune.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekuyakbl.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3vrhwlyxi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ancrfjrj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3wkaqtrea.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3pmiylllu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uxjybivy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3csbdamqw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ihhqbeke.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3vsantilx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hqkljpic.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tdzcjnba.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zfhsbddv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3colicaoj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sxpgsfqo.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nhzqhiqx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3tvoqtwmk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3smdpnnsb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3szbkfpie.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ewcyzlrc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ikodumwd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3outphyrv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xqmcafzf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yclvybav.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3fwhdncfi.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3fziqauvu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3kejozaqz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3gnvuefsh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gfibzgbu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zkzbvmmh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3qxqgkzxb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3wjwsqyhu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3dfcmiweg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zzhcrwzr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3sfnmpeks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irtzywnj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3glguiusj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uodihkqj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tjedxkkf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ntaqkzwr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3npxyclto.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3qobjykoa.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ruwhnsht.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fzbvxbkr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3gzdmotxl.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3pfkxchog.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3xplulgct.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3rmypbpwg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3domeqcbk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mfqcuklk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rjfjkmau.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3evopfnnj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3miqrsprh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3degvuteo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3fzqtwscd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3phtxowqk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3eeoaiybi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3owbzcogn.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ubtplllh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3awknfjsz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3srgwzfzs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kiddycvr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3xwihgaiq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3noljwsaf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3yjaxweui.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3irypivod.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3armhhcqc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wmkoavyi.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tsuijkfk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jrvkdjzz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3krbzegjd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jsxgoyln.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lapypafr.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3httsncve.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3uwkqtwkl.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3lczutakr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3mqkxjddn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dzdkaylc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3lmdypukb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3xciwjdnq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3nvdymuit.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3msqghndm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ggtjfdyw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3dnxzwpqm.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3olfsewgs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uyvewjfp.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3btrlhdkw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3yzsfomyk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3bitqplul.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jvfimahx.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wakdufkw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3cgagvwin.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xikwmwlh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3lnyrrexr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qwwqlvri.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jpbtrivm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3pmrgjriq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3kzkaqmjg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ixruwzvs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zfcrpich.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3akpwpyta.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3daznxiwh.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3oamwxrde.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lefqqdwm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3vtenmnan.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3chrlxlwi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3zpyxnjbk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3acyzavcx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yfumisvm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3gjxaxwgh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3trfipatc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3qmiiybid.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gczhgmgy.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jbwzeagr.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pkjslhln.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qqvzaxnq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3yzrmrvmy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3oistswxt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bgzjwgtw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3nnjdudpy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3dgqrcmgp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tclzlatd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gfykomnv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3jfkgjnuv.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fuzwqome.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uswmgaov.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3featapgo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3oevywyfp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3hykcelbf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtamrwiv.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3mdjsyaza.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3incxztbv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3sqamepfq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3rdvunobi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rlzkehsa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xlvmsuto.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tanjeobj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3tpebwbbo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3fgccpxjl.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kisujbrm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kxbxjtol.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rpvkbttj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3orzadiso.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zsibgpsn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tsswnohw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tfzceppq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3suhyrsox.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lgehqhxl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zhnbjvzp.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3lumdwuvd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3aupmotsl.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qrcsytku.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nbaqkrba.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3hormxhei.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gcajwqid.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vgumzpba.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3waqaifjh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3rlhawqys.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3zuoqsbdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yeselwfh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3igmsdxve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovlngphy.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3bobqardm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3knkxxglk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3coiodwnx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3huoromhd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3eqvwcxxv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3urrxgrwi.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3oskqeist.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3dvrlgdys.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3rgayqjad.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3arhkyboy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3osxpeumm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3rjyafnvs.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3bhkpycro.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3hyzlmwrl.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ybevjsth.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3paujhheh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3tpqdafjc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3nmbvbnrf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3enshcfti.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3oelkyqnc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3vatjhmot.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nmbmqsqy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3bntcmuwa.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3jtdhbito.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3whrzzcoe.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3hkfuqhhu.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3httgukhd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3zhpislwu.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ezjtusmt.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ddonxgzr.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3fmksntgy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3txdarzyc.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3fmddcvqw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3hrimagym.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ovjoiltn.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3luwydjci.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3tajzxhds.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gtxrehte.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3jywrkilq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3sbqilcrw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hqcvhpbc.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ahzgauan.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3nonvcqsr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3vydahrtm.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3dairfrfw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ttkxakfe.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3aofsfpqh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3suohludl.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3kpdxfhcx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3hcwsvvmr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3zpdzrtuj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3tzvqbgvu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3fhodreme.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3bvdkenuw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3azlwnuru.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3vtfewuig.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3uzmjrsyd.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3abbwtopn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3afhfjvpg.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3awoyyftb.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3fqvqcity.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3cmlkrpfa.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gosbnknj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3issndfmg.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3jyyfqcbx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3tyzgaxei.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3wqcremqe.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3fzqpcbvd.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ltxowsnn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wblehusa.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3kuslehvs.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3gknfpmph.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3psaoztpy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3foectrgo.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3bohaonhy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ybqwdrle.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3dbavywnv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3pvhccitu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3kgqcmosj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3srpidjve.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ysxcviaz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3risijntj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3hwiuqvvk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3bgzhvxup.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ndcawbgz.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3dnocxffi.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3osxchclj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3iwvmfapu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3glfowmnq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mqdscmpv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3hytjbnic.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3atakwrqn.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3rlivihyi.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3tfzeozfb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3zzrfesww.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzfvnwnt.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3rpfmovvb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3xnwbodvt.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3wxsolont.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nidcvnta.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3aajibqox.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3webitaoy.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3npfcpwav.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qrjgxtsj.html


<!-- 参考信息 -->