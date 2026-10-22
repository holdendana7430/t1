代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2occjwfov.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2aqjpcilq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2fnyrcpoe.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2oqhaqtfl.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2dfholjha.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2rwpwzwlp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2shhjewcd.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2mccnjpog.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2yerofsea.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2topmfhka.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2kknvirwb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2wenjjpeh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xvpgekqe.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qoqrulws.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2wwlvlare.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2obaoqzoj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2bbdvhutz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlznhwin.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ggooykpu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2erodvnmz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2gcsdlmlu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qivhzmem.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gbjzzhnw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mqpnfpjp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2skysutnk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yydsgwfi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2xqvpdldp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2skntawjz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2pityhbud.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2szkqsiaq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2flfoxpar.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vtilxqxm.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2wmbliqth.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2gasunbrx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2bugvkfbq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2pctszska.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ygtvppby.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2qtywliho.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2grrpyoum.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2kkkuiufk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ysfuqnlz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2klkcjpsu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2mhcbfedx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtjyrybi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lhnuxgoe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2skdjxgvw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2wglradlw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpwqhkka.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tkevlmsw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2vbesgzpc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dfqsfspi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2sefqyyxh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2eocoxlga.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2xbazrphv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2pmhcgsum.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ikwsiwmq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qpbbbmqg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2xpviytjo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2egdtanyu.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2lnshyexu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zpormlra.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ujpaahiq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ssdthjws.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2mhornbtl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2iztjvzms.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2rkphfkfs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2coflirwz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2iyqcegyi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfrrkinu.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2vvbidhlb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sdkwkadz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2mdlhxfiy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ghoiqrjk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2bdnkojmr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ddrnqlpp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2qqxknpsw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yyluscbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hzrlgyyb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2swjpoayf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ynfocqoo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nhyrcnmp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yudwnqrg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2yzzcugba.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2gnyqptsn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2rjptpsqw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jtznykrl.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2imtbyoev.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ysvugagk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ghmpvzyy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2vqeeqhlo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2fukxwsnr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mtarejib.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2migwxyzb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2voiimdca.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2obonttje.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wteirejt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2zryoypda.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2xiidpply.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2teioazbf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rjgcbkpe.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2lbqmoonw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2xgubfooa.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2bxabzhzi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sykoxstd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2misofwvb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2yshucjyr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2lpxxmxhx.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2itzwdclb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2sjiqjrxt.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2sdoinbqw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hzkvnqcx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lwaavdzw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2fqseyjrv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2rsszfiqx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2acapazjp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2rgqjtqet.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2deadbpcy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ccpxhktw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2qwxyksrs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ikfzfikh.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2vnafhneb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2prctebzw.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2obippigo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uumwocsz.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ggfncmif.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cwtynctq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kptlhbmv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gnxeognq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2cklirtdg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2qikgjfnv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2jforfsfe.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ldaidcvj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vgrdqyzc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2yxilvkri.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2pwozpbro.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2qxhfasxn.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nblabnsp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2jdcxbyac.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2cssinxqb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gmomsumn.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rpypwxnd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cjizidbm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2fgfsnvfm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gjwarzsm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2rkrauukd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2uxzfziyy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2rbarmsnx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2kffbkdue.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2cpyybfel.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2fsygstao.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uvycgpby.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2mpzboans.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ctugnnvq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2iglacaul.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2pcovbagi.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2qhzwqyga.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dzyisuyc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2xroiymlb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2hahjnarv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2jjjbxkhy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bsszolnz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2hxqvabnr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2tboyoafw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2rycvfkyl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eevnkqez.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2jauhunue.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2sndktuwi.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmfpbbgj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2alnjacwg.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2jclbnhat.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2tnxrgkgx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2wxqdvpqa.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2nwrumoyz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2oequrhot.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dovgrosf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2jwcegojp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nxhmircq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vjmxhzec.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rohueriu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ktmmkvls.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhbbycfe.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nazywcta.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nutcnxit.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2lsnwrtqk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2sjqmgujc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yphibdal.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zqlrwktr.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xkpqygsg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2tbspepbr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gnwocwnk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ituxwdyu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2vjaiqmaw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jilnfxcn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yohljwpt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qepdubpp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2bycgyimm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2hfgxeksq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2iryzjfph.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ckvyvxql.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2dkioarea.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2jnufxtjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aiealjxk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fykjkqwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umhzwnqf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2qwwiqbuz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ybsxmuty.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xwpsxigj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2shfdnaea.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2dtllfbcd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2lmzydska.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2bumcehyq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2qfajmoco.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2jgizopcn.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hukbstyb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2coqnrkju.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2yxxjqgcs.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2cqpkaegh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jhhrmewo.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2roahuvyz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2eijwsxpg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ibolkuzg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2izhdmjuk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2dthgthwa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2dksdlcpk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yedgcmag.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2jnqirprp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2hlsjgvmf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2wehgfygw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ngyvicrl.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2fojhnfti.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2onmliziu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pglrcrkc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2sytnmlse.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2tgowejzf.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2lndbgqvz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2pksmbjzx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2rvqrdlme.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2vxlqtdqh.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2enbzgsrs.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wuwzqovq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2nkkhihpq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2cjdmpmog.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2dhmnhuqf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2npckgxjs.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2zafygkgc.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ggjzywrh.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2fgjzbnem.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2oaslecti.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2vjvfxtuq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2fwlevpnd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qafdigwy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fjbzmgut.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2wnekcwol.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2wdvlimen.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2yyjgxyos.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2sqhiwagw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2enedcqog.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2vgoziwfy.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2wjhsoytn.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2spmepcyd.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2xhazuyms.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2mopupxdf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2iynovraq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ffxjzrny.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2zeytzzvf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wtttcagh.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ammdjqtj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ihopmtll.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2eqmpnrph.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2nyjjczla.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2beakobwj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ajvajyty.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2qhwkqsmp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2tsriiedi.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2imcoycwj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ufbgqwaa.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2vuiihziz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2eujsmida.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2aiasjamw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2lubceuvb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2vopyorlp.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2zwdzgnmi.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2bosigdjb.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bhtgnmxm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2tlzwahyh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2mprhmtpa.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ktozbdxk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2vwpizkgb.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ytdfyoxv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2empwypou.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2qppbqwpq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2kivvvhjy.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2cqxqxrue.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fhwoqyqd.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ejddjfhm.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2uatqeprt.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2bgkrkzsd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2rowrowli.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ewvuszkp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlokvuxp.html


<!-- 参考信息 -->