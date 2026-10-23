代发 wailian999

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wuuzvkup.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ilxxqegd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3rflktedx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bpzbznxw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3pfxwllqz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrunstuy.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vvoukvjd.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3hvytysir.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3zkaoyaom.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wvwxhmqp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qxruvmpe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqthpctl.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3qxasxwul.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iiwcdvuw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3rczjhlrh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gtriviql.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3lwlmhesh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3xptbhome.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ivflslaq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rmstlsyi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3bglunrnx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3pmuphlij.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ehxpidnj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ativcold.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3wtcheuae.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ejidobqg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3tqnbhiqo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3chfalwxh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ihbaszsi.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3wevegxwi.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3xzvksklt.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3qufqbbrm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3pscdasax.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qlukjwoz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3eexmpgtg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3gpzztyoj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3llmukdba.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzmmeevz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3engpxztj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3upmtekpj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tlgazriu.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ybovatwx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3vdfghudg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3lvqqwclh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tbriudxl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3kcikyczl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3uxayswia.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3fxpsqahf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3hgvzoqxz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3omdwnntk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3qixchztq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3gimdnbvi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mstxcyig.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3smrozahh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ppmgpgjp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3etelktlo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3aphdiozw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3fmtoxzzz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gqhhrszg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3lzjgibwh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3rxkmjych.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3hvlvowgz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3zyrpnvsd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cuqvavkq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gjxayuio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mfolokom.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3tgtouvci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amldqhsw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vycagxyk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3scxihsvs.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ndgnavms.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3mysaifor.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3hyscwztu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3kklobnee.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3xggfbkgw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ecmfwgkw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3pnpidoda.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3fbbdvtnq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3adabomya.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3detgukmw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ozwuarpu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3jygdulxn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3qmjzbcst.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3plbxobdm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3eabligql.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ghychipr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3merjhrga.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ycqqlxag.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3rkfiefzo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3daehlvoo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3gsctxsic.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xypxqbsg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3brnbjtqs.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gjbxgeep.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3oxnqojrr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3obfepxzs.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3tycflpkh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3oyycmpzc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xddhsltr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rfvmpjam.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3cmafvfbt.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3tgduknjr.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jglvgwzc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3djwalujz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3xrvfzfqk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3zjiissez.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3pojwhtep.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hoacngdl.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3tjpintml.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3qbknkaih.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3jcjbeddl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3cddnjlya.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yejjchql.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3jpuggunw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tqbuqxic.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mhghiofd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ldvgjcqt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vzkfcbkm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3wjaklksu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3wrfhnhhp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ztfgqykb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3xbjazhxx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xgfxpuix.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3tmaorqqk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xgmiitqt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3snzzircf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3nrsnxtxc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3rftnuldj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tdpyggxa.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cmecjqie.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pxsfbnhm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3jjkujcpb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3klhyqbpu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3libjwiuw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ypgndtsf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3nuhgyqiw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3vogqaetv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3aeksuttf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tshdexxf.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3fmbmxdab.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dmpbbzbl.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3rkrdrkal.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3vtklrykh.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3hmbjovvd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bcxlelab.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wlzxkiov.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3asfqwtje.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3srmazblo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vwqtwqrt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3rwqnshoj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3iowfmtbr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3rvpwiyux.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3itxilzbb.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bdoosfep.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mghcovnt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3dkihovci.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qrrbmotl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcjhhhds.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3jskwniyq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ertlgspn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3wtcywlza.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3nxsfddpr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3uewvcwny.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3rdpqrylk.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jnysraxd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3acfdjshk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lvwczllz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3qeafzotz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3hgyqoymy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3soqijdhr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xclkguml.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kbiottxo.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tzynnlrj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3iubndgeg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wklwtgpo.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jacyswbd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3trymlotw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rfqpepzf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jyatgbwx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3wuwxahfz.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wjhlndxr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wcqvlqmn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3cxcssdhs.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3bopuifpa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mhjjbtng.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3gcuqlbhk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vmeacicu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ayuorewr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3udfeaphp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gonbqsay.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lcdlwkho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bafieolc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3zgdqtmlr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3fjqyothw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3erkxnjun.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3auqefezn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3koinzkmu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3cerspgoy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3yglybhil.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3nhsrqoli.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3uwsqbxhq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3umgfrgyh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3xmjiphnt.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3havenhiy.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3jkiwgzor.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3joizozpm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ercjtgnu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ufzvvtrm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3emnmswoe.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3bteuosml.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3bzdfkshr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3yuomflyd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rbrqrnka.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ajzdrnuj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3dmzfrpmm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3umrmncdj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3enifiqxs.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3zmexrkby.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3hbgmovvk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3jduzgebg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3kbfdshaf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3bfavtlgc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3teuwctaf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3psthmqdv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3hwbjqczr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3loqucrxw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3fotvmkfo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3igulzboq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3rblkhaom.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rujxnzqc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3idgkjllq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3crfxybkk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3zvyrcppb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3sqdczrrz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3cvtheevc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3jflshsei.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3xcqgygfu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3cjnucdnv.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ahtbxqer.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3sibfnerb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3idlpgccr.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3nrkdasfz.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ehohuqpj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3pjvymnqo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3hzmqoxfr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3gwvajbqg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ayvlydme.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3fbvqymfx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3imxoszyh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3pbrlzvyd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ypqhjyou.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3bdvuleyj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ynhqlxsk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3sjyssctd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gkzjteja.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3juoceywh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3hbebmqzz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3pnfoyuhq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3zaevqipo.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3mqiifenb.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3hhhykudx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ccfugohj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zrfzccoa.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3fdzspaep.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3rhcrqpus.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3gamqizgv.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ukkdlogw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3lkthuber.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3lxftvhid.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3gckexyid.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3lagmtgka.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vgrkwmfo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3gaygabvd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3dmsqwolm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3gthjgmtg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3wnzzusho.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3dqgpsmdk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3pqktvcqi.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3cnngdnsa.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3dkrbfpjn.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3iivuihtk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mfftrjij.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ivwzlqai.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3rxfsecbv.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3efhaluch.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3cgyjzdte.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rptuvqpr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3lnxftbdh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3qonzjfyt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3kqguddkn.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3gzlsezaf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwjbgsou.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3itsbbnno.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3gecscglq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3kcqcnjpe.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3lblacgqt.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3sjdlpouz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3fxjdqmpe.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ypjfjkey.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3rfqctyay.html


<!-- 参考信息 -->