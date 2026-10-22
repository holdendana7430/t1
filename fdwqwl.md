代发 wailian999

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mgyhndji.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2idzcxoun.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2dmtxkbbl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gfcysupi.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2fwgbhbnw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2caedcjji.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2pesklkat.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cftuuucd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2dkhmscuq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pywrbtuo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2mrrmcxml.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2iuugkowf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2cnwfamwa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gjmvfhmb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2rqsrfwra.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysqlixqe.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2sshfausq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fpmdkxeh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2jccsfaxv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2adwlfquh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2vxwjqyti.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rtometcc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2dlijzjdy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2stotztyi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2xjmttpbq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2deqaupmr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2mjzvmpzt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2vvydaybb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ibqucpcj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2huwyouvy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2clsezkdy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2gwsdptkq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2nuscnhal.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2rvxpicfb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2fvshqhkq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2npcaiqxo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2kazvaoof.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2rhfybugl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ffoeewfd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2gcrrvurp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2zwycmiln.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2icrmxwjt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tcvqpmgm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2hcbjgosn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2yykpxpul.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2kjovuiiw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nnewxukw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2vkspvmsp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2raargmcx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2mlcjcxjp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2wnsbwazu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2zebparra.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2aogophue.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2zezntzhy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2kcwynsdx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2fwdqztwr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jlzgqvms.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2bvscgvjy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hgxnimnj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2vhmbayiy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2woxcirxp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2cuspcade.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pollvwcj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2wtageoyl.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2tvghmxfu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2slhqxabt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2haztdksf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2iobnnxvh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2etinyilt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lgdgdqwx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ytzlqqlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpkjyoxr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2amvjfkph.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rgivgbhm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2dzqgwrmr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2nwgvhaph.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2affdhaex.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2czlqvsmb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2smiqlyil.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2shuyiuku.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2xmshqgtu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2wwqativo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kvkhqohm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xfeaywcr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zfvmdfcf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2efdyxepy.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2kpolsoyz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2epnypzgb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2bklbzfal.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2zyfxjwya.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2kagseusf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2toappkdt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2jxgmljql.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2aklvfqoi.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2aatvplqg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zmmkdrfk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2tdfnztwe.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2aowflnsx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cqyrtpko.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rshzthfz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2sspnkgcj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2clmxrjbv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uxujvxws.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ymdveksb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2gvzzrnck.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ceiehtbb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gdrekxwt.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2nnxutttj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qjqivfcg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2afpcwvtp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2mfxzcnug.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2benscgmq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tyjforyr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2qzsszneh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2scuglmbw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yzlfygcr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2cktdxqjz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2wnoxpnbo.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cqagslsg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2txxxftgw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2bmafvqaa.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2bjxclgwr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2mqofopcc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bdpnsmuv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dzdxpdyi.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ylvmwrcy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ycbltzzn.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2dfperesp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2hspnacym.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2znnrecma.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2epcrsutn.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bmbxpgah.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2verhdlej.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ermkrwpv.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wieozgss.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2owmoftgn.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2yoougkjo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2nybuapqy.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2voahvwtb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2qhoartle.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2kcwvdqzy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mvrtteim.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rcrtiajd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2zxtrdxjd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ggjfolpg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2lkxmvlwt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2yqmvnhif.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2zxxiaubo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ymshdphl.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wqiojbmw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2jbgackra.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ywdyadkn.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ptagerqf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2qdlnhshw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2fjblmpxj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2sjgfxnbp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cxbmysxx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2yjusbcgu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2hmzytnox.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2jntmjafl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sajfuvdy.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2xfobaoso.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2brkrhgsy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2mvlvrmwk.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2bngzzxcw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2jtsqohux.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vrvyvral.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2kaythtdz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2fisyanof.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycbniayw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oycbuftt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2tdrqzhjc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ibopaluo.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rjwucxkf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jigjxzpf.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2uuopdtfo.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jxsnnwli.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dshuyauo.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ejfqoqax.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pzqvsszv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2xxyjleku.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tgguqail.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uxlbewsu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2rrotorkp.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yenafmur.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2algvfeob.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2absyfxje.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2efcdivtp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kryjfhcm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2zraefilz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nopwskml.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ikjssuhx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2oinaynyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2evcwtgvc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2efdloebc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ztydlkqp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2uqdkjrzf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rifzzvbh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ywjtpbbz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ajeplhox.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2pmbuyetg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2guuoaunj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ncqwwmnl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ojdfvyrk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2rlkhpsib.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2oxgdjmua.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2krupswxy.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2todllshy.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2qreuknto.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2kdvjzrzj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2dwssvvhw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2xltrltba.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ngfrghwv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2qhdampml.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ytvyocev.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2pyoemwgc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2dpnzdorx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2qhnfkvip.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2doxzsmva.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jonjcvmo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2jiyrushz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2eybwfnof.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2kesqqbrg.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dmrvdrkh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2czzkydlz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2vfdvzdnl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2odzxezhj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2simzqrbg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2eqtcelxz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2jcswxwcv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2jmxxdjmz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vyrmrraf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2htzuupuh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2vefcixfk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2exelbhat.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2rluztoec.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2tazylfru.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2idbmxkfb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2jetcpwzm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2whzqkgxa.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2agxtbgok.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2emsxtugi.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2tlvbythy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2dewbyfwz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2prwngzta.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2qsfxxurc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2yxoqhpfc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2zmoqeemd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2rrwzssne.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2nbbtlkms.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2vplwerwa.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2xuqjembh.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2zqqlrkeu.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2qciyysyg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qnotahaa.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hivuyscx.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2hsqvecvu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2fzlskwbd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2izthqlvn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2rtbggmbx.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2pzjsrvky.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zqdjxsqf.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2sbklvmez.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2atymovwe.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2bgmocina.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2nxtxamto.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ihnaesth.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2cenofcnl.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2kjqvrcab.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2nrknynty.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2zjgqfbhv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2jkjrgzrb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2dyhwgxwx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2yuzittxl.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2vlsaavoq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2emstvcza.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2fxobzyxf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ncawekdr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2uzhbjjva.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2pecuoqtm.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2frqfddnl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2gftcbdjo.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2oodjpwop.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2uoppllrc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2kkohckuw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gwphjlhi.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2guivgauo.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2jadiktck.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2chbkmufw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ayjmcqtu.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gmfwomfp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2polsjspi.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2bbaftyas.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2wwxusljb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2uegzljbu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2sxosnmkq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2jggrzsgz.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2zupfvunm.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2bsmiyjal.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2pmakxbpp.html


<!-- 参考信息 -->