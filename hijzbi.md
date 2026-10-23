代发 wailian999

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wbhpqeqk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3rrslduww.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3nggsgdng.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zezlooxx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3kzbdcfzt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjayxgfd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mlgchmzw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3kxxvjewt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3hieairul.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3osgpscpi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3pptwnhtr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3vmdncaoj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3fsbbwpoa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jgjhlzis.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3kbppvgzc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3stapusnu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3tgypzlof.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nahxuyfa.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3cxgxohrl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vglnvbgl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ctoshhqg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hapedbej.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3qpuifbip.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3itkyuluq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zzbwoucg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3yhqhmqcx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3bcqividk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3cuorgooh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3deeflgiq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3pmdecbwd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3fteuxlln.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3eaxrmvmr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ymtbvecj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3zvztclox.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3zjpsorrr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3oolqupov.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3pqcesdxi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbbepoon.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ntkempsp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3njggagyb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ivnineas.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zwdyjoqs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3elsqvhkn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3lmoanvqp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3knusmpqf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hksofkap.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3duoitgbr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3yypudijt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3plzpojew.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3iwbkaprw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3bxdroqpp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gznxaiba.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mhfwleyg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3omkockfa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3wotrrwrg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3patefvwf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3pzsaksxv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3pyzjdcfn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3tonvkhzd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zmdchtvl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vxqodabn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3enejcdax.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3davbyfvp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3qrwleffx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fprprqgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lkmhcflu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kxuujxqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kdhfxfgy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3txpilyfi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iwifjplg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3goupetaw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3watgpzon.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3bbngwqsh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qunghozu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3wuyqlstx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ysrhtluj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xceviynl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3uvoqkfcj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lcxgzdni.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rkajiqyh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kkkjcaqr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ipacptaw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3jjbdbfuw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cztgyzae.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3vfrfgjnj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3bnzcvaly.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hzgskbhp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3cjbyhgcc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3odxsovio.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3hfxyiirg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3bofbvvuz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xjwpdwsu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3qdfkmugp.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3fkczssau.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3awbfsexl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ltmcdcot.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ewwfbrxp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3iefpbytg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kaauqeji.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rootqaxr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3dtnzruvx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3egwnxrfo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kbmesqfj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3nrwtntzm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3cvkzunux.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3nvyevnjl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3abpupiyh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3dqitnsfl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3owqfesfo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3teykemnn.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3wkvojenq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3pnzomxdy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3egniwabb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3hkkijfla.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3uvgicgit.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3meirgjxg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3czxnvpmn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3gboipnoe.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3htfvrwci.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3wftawrjs.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ycwhnjew.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3cxvcbvdf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3otzvfnso.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3wrzidwbx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3letfadvz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tdzdyyes.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bkvkkria.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ytvckepp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mfkfhiqh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vkkssgms.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3drfrqxsp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3fnlxxzjz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zkcdlduw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3uooylgil.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3gktfoopf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3hfdleeit.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3gumhwixr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dimhrpwy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xvwmqtww.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3wjsuuixh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xtexfkiy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3hjyuwxon.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3nrhbtzfj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jgnckjgg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qvtqwxeh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xjbradsd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3odzvxewq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3eavmzrkx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zwxexyik.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3fvcmxugq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kseeqrjp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3uzzknxyt.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3stsfalne.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3qvjgtmgg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3xmzlhgrv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3udbflqrw.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3haypwire.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3qfvtgkie.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3zdobwrtj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ccmxmpcl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3olruzlhg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3iosiuaoc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3oyturkip.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3yckfhdsl.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yuxxvlyi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaaibgdk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mawgteng.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3zmidxcpm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3eclucaig.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mahddkle.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dnqqdiwj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3diwffnyh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3oehmvwmi.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mwmnjuyy.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ytmrnjum.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hyhvvgbs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yxcmlpde.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cyaduzji.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3cntopqvt.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nxzltjiw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qdhjgxsy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ypphidum.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3cmsjkcxm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3daiwmhps.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lslauids.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gwprlvrr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3oowxmqeh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3kwegiobh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3wmfvwlyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pnlbyqor.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3aksxkdso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3azpganrw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3opessfaq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3vclzwlbj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3tfxbgnsg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ilksifop.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3uqjirbdy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3apqlroqr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3yrnmhyzm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3bcqlrnwz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ilbmpmjk.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vnyahjih.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3rxrmiqly.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ovomivuz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ybrczvei.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3tzrmgsnm.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3lsfnbkgh.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3oijnepge.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3utqulwsn.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3orbxiljq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3kkcrdgnv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3eaiaqwpd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hdchybbj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rewkdamd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3opnfizzg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3krjljlve.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3mmffsqsi.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ejlxtaka.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3sayzwrvi.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3tstfxqoq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3eyvvdchf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3bqtttpnr.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3rwcdxjun.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3hpgpcvls.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3trsybfke.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kqavjkaq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3kbabyctu.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hlxmpksg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3tjkbwgef.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3vnucxsna.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3jipejbjr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3owdidxcb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hkqtjsjs.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3xbhdrdyd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3xqrwlbeb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3owywytbf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3scjdhgia.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3gykluahi.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3jxmopfti.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uewomjmk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3eenhkwkc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ldhzejmc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3fqjbhhmz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ynjmjjtj.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3sjttuwdg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3pkkxleso.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3irugejei.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3wjumrbrg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3pqikosnb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3tzjgxoth.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pxbwmjvx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3fjglnrwf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3bwfufpdz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3nyeaujhp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3zcrqsxzz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3lnkxfoil.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3wuiipkzh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3cntozsfo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3zzmhaqpk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3hrymzvjp.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3gavihoer.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3qqizlexq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3safwqxoc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ljkknhnb.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3nnvxxdea.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3errgycrn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3fahixygg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3geujnxci.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3isailocx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3bkbcolvz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3nzwywscc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ripindnw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3jbvwsumu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3fncdpfpa.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3dbqyscyy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3gsciyoso.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3phmfzyya.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3tqmkbdhi.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3hcsxunkj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3xmvjkcww.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3yinloiil.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzemyzvi.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3kpmpgwgr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3byrfvydc.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3nzafockg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ukigtjoq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3aurxjxpk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovbrxpqa.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3rjaqdibg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3zuwbtqvf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ckklbzhs.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3aiwvtfwe.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3xylmcdoi.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3pbkdftfj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3quchmzke.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qhjqtiht.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3qiratrfs.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3liadkltd.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3cmaodmib.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3wrttsyox.html


<!-- 参考信息 -->