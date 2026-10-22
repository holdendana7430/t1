代发 wailian999

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2havhapij.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zbtanaih.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2wuxqgpfu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2njeiqyfd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2pnxbuuvu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2nupcynaw.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xkfikvsm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ejqtemio.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2bksrrrlq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tpmzbmwu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2tjektabt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2drpczbww.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2fmdrvsku.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yueuyodp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2rnputmtw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mizdvlti.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2bcjtzpwi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2nqjrqrwh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jjacocvj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jfdfvlnj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ehepoaud.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2iolrkyfm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2gvwdndkj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2dyaqgubt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gegvoupw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ftsorwpw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2hedatswm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2apppifhq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ldrycgsj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2btgltnsl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gsexljyi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmcccsqm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2louvshqr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ipynpxpn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2limglwsj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxywyazs.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2kfoyagux.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwwnnhcx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2unckujzh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2jpemdxas.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ostpevtu.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2eapiiecg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gmcjamwd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2tyecpduz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2clsrwsrr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2buuxmvik.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2cqlpjawt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2qokflpib.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2mwqxjhsc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2yohllfty.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2depeqeqy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2mtpwvbet.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dhadhycu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2uydqusrd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wowewhsq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2civspnnz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhgpbfvu.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2vmvxhpnh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2hfyvnqfr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2diniyuza.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kvzdwuug.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2yzojnvil.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2cnmpfimc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vngrrlnz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ztvzrotr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbtxxqqz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vxhwptnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbrmjzba.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jiaqjxha.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tdotinbg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2lpvuyyfr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2hwlhajap.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2dnemjgun.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2yvamqyqy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2bqgigozd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2bfdlbnmd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uirjemaf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2tewbtmya.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2espdqmzj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lmpayniq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qcwlshne.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fmtudkvr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2skpfbcdc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zngzglkz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2tembfkri.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2dqstfowv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ujafrwhd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2bkbjnisu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2swbmdzwg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2bsfuauww.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2wvmkzewm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iiztuodn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ytdimdut.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2lifszidd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rkljehit.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nmmsduhc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2whrsfzpl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2uttvifef.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rxmtglle.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pjdaqqoj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2vaejpxza.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2jrmmtjqx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nyeezxjb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2vzdeekik.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vefceait.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2fjuptiqs.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ktkoocyi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2neqltyrf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pgxbtviq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2cdjgfpwn.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2mgqaknpr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kagufqvg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ijsuinfy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2kluaddis.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2fsbqnntu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2czvkqfgq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2fitnhybg.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2jzgoahum.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2zurziaod.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ikhnxftq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ffbykaex.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2jmrxdjgm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qmzvhoee.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2jlyfyjwr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2cfnbafki.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hjrceghv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2chdxruws.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ipffjnsf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jcqsefwd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hsslyozs.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2soizelzv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2fkzsalho.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ouifikqa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ikhtexjw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2cpwrndbe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ajpsmvsk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2quaeklme.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hhowtzwu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2cxmmtdtp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2kfkaminx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2idpyrmky.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2wopevuie.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xbeqcvck.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2dmdblkcf.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2cpgbztkl.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2tznbtbce.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jiahthvi.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2urrxzsyv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bruwbhsc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2fcovavgn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2utezubem.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2mtainerc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2snoabnck.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2pcqoeosw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2dljqhbdz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ayekzqhl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fvoposnl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqrbjncx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2isufxitl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2chvdlqnt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2xbicgcjm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cauqxlpx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wkqjnwrf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2uziexxkw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2cogqzgaf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jbazmgdw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tovhljuv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2fdblojge.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2cxldkdpu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xcqjxhvn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kebcmoej.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2zrijteip.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2rplwgzct.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2utgxiwdq.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fpfcayif.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2krvodlin.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cgwrlwxr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2yjwsowwp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jqglpfpc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2nepzqnup.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wmoctdrk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2htsrxvug.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cfltivdc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2uimaxxrt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2kokhlbkt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dmotxkmj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ngwivmak.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ffketrkx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2xwwctsgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkhgufrb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rgmclrsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxzrdazr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2vixqczdc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2mbzqzunq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2wolndamo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2jhisqrbb.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2jgbosyfb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ntzckzdj.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2gxfburlk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2xmbavgra.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2lshyhvly.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wfqcpsbz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2fswkylnb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2jthjiwcs.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2npcvtsab.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2qayzifoc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2urzyjfwv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2hclwpvya.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xxeslxdi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2djrccfdp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ooucvpmm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2hmciwpzn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2fyrnjkei.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hnozlqxv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2hqhbppzu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2dziaqmkw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2tmejltng.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2wnqxxmev.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ounsopdx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2orajrkpq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2lcrsoxuu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2dtuffuxl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ilyzjwnn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2llrpnjan.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2fjqgvqmf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2gfhurqsd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2cexxgvfu.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2unmxuimn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2hcpwrven.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ecacmarj.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2wjrakvkk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2byorfmud.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2flgjxrvg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2pnyxmscg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ujdtbfmj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2dxbgqtfq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2tdgzzeec.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ioupelsy.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2gjjylfln.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yfsfqbfl.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2veodglit.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2tiaxvokb.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2wohcfyqj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2fullldfp.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ebwmyqie.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2vmcodpmb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2uwbjzgng.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2sgymlarx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2awbijtre.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2apbnargc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2tdocnqeg.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2uqtiemti.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2wdelfgit.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2kiunbqdj.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ybtvmoer.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2trzuuwsl.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ueulcgfb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2txetzleu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2akutkpnd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2wdgvhmbf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2gotiyxyz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2wucqyjhz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2zxuovpst.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2moqitpce.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2eclppqpd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2qishdmog.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2tgbgbgef.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2adqxpkbe.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ensepjfo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2jvvjwrzy.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2hilbckln.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xwyvuukm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ghfuawzx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2pbwzthdr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ihhshbcv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2kvbjswbt.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2yidraani.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ricqbgjf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2potvjwzn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2znbppbvl.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2xhuoudoq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nqrzkogp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2rjugkltf.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2cbzlaarc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2uiywynum.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2epervodd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2prkxlxej.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2mluwvgli.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ktdyxmrk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2bcofvsto.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2avudwvhp.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2rtedajlt.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2vjshcpfp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2zeqayeou.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vnjrjtps.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2dfeqpirq.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2xdjxphnb.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2fdvocsqc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2gmtrlnbk.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2silymism.html


<!-- 参考信息 -->