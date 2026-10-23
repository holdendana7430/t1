代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3tpiwvuft.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3scnsxttl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3aupjlhip.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3npaffija.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ipxdvkzm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3hyultskd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3dwzsbyde.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3jakdflfb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3sodfbqei.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ujayyjpa.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hnqzcrgk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ucyyurav.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3twzdgimu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3cvjzxxvg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3jtyxljmt.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ravyudst.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lrfxuayt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3oktnyzvb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dvnwaqsi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3drlfcvwx.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3kkvcyfhh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3fmcltgwo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uusctljm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3tmlhcoul.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3rrknpdmb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pujumrjs.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3xqmwnxyw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3grxpciel.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3jexedijk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pmeljdrb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3voqlppiu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jmfkupkn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3sjgjnalc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yfyyzhmf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3iyogqfks.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3deghbmgw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3qjlwvfcv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3dkolbsnl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3tzprlkva.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3mzxejcyy.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3racrkdnb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ketwuyva.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ywntofzd.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ufgdoyjo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3czpemhqt.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xxnoiwrk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ptjfbgbu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3exkhraqc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gblvfnun.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ahhkztal.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xujiaams.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hzudzldw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xaygzaka.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3sumqmcdm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dsrphauo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3lhtfnivn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3tiqkcclv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wklbgqvy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tadicgtl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3omdeckzg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vafuprpj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hhxbbyvy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3tbtjefda.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3xcabcqdp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjjsedey.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3mtocdjee.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3shsikzzf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3urjrzmnx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jtqchaoc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3pnjxqkbk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cuhhvsjw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ucvlxnhb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3lnjxbuzd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3mwspcxax.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3admoghwx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3alaamuze.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ecbddnik.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3xztdsakl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3xobnfzqb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ekfizdrt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rpkyyqwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iiwropur.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3evqmrcdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3krfdipkg.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fomkeitc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xuxerlgy.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gclzyrvl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3tqrxngwp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3enrgqdmi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hffnbyvu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3vlozryfc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ftfoxhva.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dnxmtnmr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3otdrfmnt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tidqcykr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3czuhdrmt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lfstdknh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3abqjihba.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3phoxjebq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ubcqkhqa.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3mqydwmpz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ztrwquha.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ksuopvyy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3zzncfegq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3lakofaev.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3tmyzsfro.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3hyclylqt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fqwmrdwa.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3koxnvpnv.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tvjnepco.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ustrivfh.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xetpslye.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ynszrgds.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vchjujhl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fttweqiy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mfwvyfem.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3zjqjjtcd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3oztzddth.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nivbrtuo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3lgrdlvpr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vghmnrbg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3whyeamsq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3badfszjy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gliykmbe.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ucbydkeo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3jdkwinpp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3exxbekvo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3blrehphq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3dedxqchn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3asboxvny.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3zwhcevlb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ctwoqsjg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3eniqdyrx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ygssedlg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3hudvxglk.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ljxlbbdz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3mwlcvrjg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3rztexgsj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zdofmlgd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3asbpjqrj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jjicbjub.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3algwsued.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bbfhxfyl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ilgwnazz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yyudsuyk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xcywknnq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3sxejpfra.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ezcroufb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wwocjtwu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3uhfwjpwy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3vlwmnspc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3kjahywbm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3bhapjvfk.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xpwoidli.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hdykgfjt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zgcklbay.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3uhnntbli.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3adukzjhr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3sjrqaqat.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3spqjghaq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rhrvhebg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qfitzmdd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3imhpnfmy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3yimfnjcd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zjbazksu.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ddcytwxr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bcinkpip.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3eduegtqi.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3apliahsy.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xmudxdfl.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3lfvsyfuh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgmjnyvv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3fgbzqozc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ovbahbza.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3xmwzntmb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3hqaqflzm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3azfwmezw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3nfxyfhjx.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3tjowutae.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3zzzffirh.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3toyqslqx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3krdzxatr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xkftipvu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3rxkqdsyl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3fjqcdjyq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sllmhstz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ffccvnkt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3nihlluqs.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3aeenlidq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3iheafffk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vehbykvr.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3piybtjwk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3vjlgkban.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hsqjylsi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqxcpxcc.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3beowxpsf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rhiaxzdx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ayehrqjr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3sbagkplr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3idoonlio.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3uraxjaxs.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3rhibdiog.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gqjixprp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3xmgltrbx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3yfdmngjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tndzbysg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vkphhyjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfmabmih.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3fzjviykd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3kdyzybyd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3bddbpghj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ywdifmcn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3alfwmdwo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3znaslmye.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3zasvornb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rbfscguh.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3nacnpxpa.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vcrbddjh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3rjrvfpxh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3vjvdlzrv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3jlqdhxyt.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3waicevsd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3gmxmfhwl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3diovhdrj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3hnlwbppx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3wkqcughh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3uzxannjo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3yjllrkcq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3vfjusoxq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dsdsamtg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3pwparvdp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sugbppbi.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3zthwloye.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3bbbmlxup.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3tgmzuapm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3qxpuackf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3qnryxnzq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ityogdkb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3jujhamhk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3jnpfeipm.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ruqztbhu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3bmsuonjp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3pifinesi.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3kihorwpm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3msohvamd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3lroxyhxr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3vmqqhxll.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3xjfrwgex.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3cpjsflpp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3tjqnthmr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3tbgeztgy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3xniwfeyx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3achtstok.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3gyahcqjv.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ancdmvro.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3umymcsrg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3xkwjjorh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3zmjzpshd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3qlwkemep.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3njzlwati.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xirrfebf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3lckoeyrt.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3dwabkdqi.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3kpygbbhx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3kkrhlyqi.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3upfgdeud.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3gqlifami.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vffvczkl.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3xxspgzva.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3zzfcxqod.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ygigxogn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3pghposhw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ujhpbrxb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3okskpcqr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3nhogmpjd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ehkmmked.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vpgdymqr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3nwjuccux.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3pxttrsgc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3qytlqlgx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3yqdxvtmu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3mtvhrxke.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3rhigvbss.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3slxempcp.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3vjqefvgb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3rccjedwn.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3mkapmock.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3rmrnznli.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3nsdzmkfl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3kffxaajd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3vxfbqoqa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3bzgbdlpa.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3stcjlgzj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3rwvnoyhe.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3mvfqwyrb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ydtgkfft.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3wrzmydxj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yyxypqnr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3mikdtnet.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3rkldeedq.html


<!-- 参考信息 -->