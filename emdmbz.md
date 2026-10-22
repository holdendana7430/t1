代发 wailian999

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2yfvxngnt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2lblzrpjg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2itreparv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2zyigsjzt.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xzxtqlbg.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2scausxzs.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2jwxzrsar.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hyglbpfl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2rwnylxev.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2gamtngmy.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zlizhnvj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2enjejtrb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hcxfzutc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lvauxvvn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2exukblkc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2zfgguhef.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2omstfwnf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2prrtrkfg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2msoizsqa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wguqtilr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2lzqnztvz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gwggpaef.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2rwcnmeop.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ylhqnapw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2unxenypz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2yamwjnxb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2vwzbtgmb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2zaiqylwm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ylmcwwhs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2urhyqfrf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ioudfeix.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rqqgckjl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2fbnwpmxm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2sqxrqvbq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2pskbvntr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2hzhtsjyh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2smdfmsfz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2tlqqryxi.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2fjkkombh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ebkumkkt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2snqfwoib.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2wwrzinam.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mzeuapez.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2bbvugwzj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2tjytsufv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ddychtxc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rbqeavex.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2kadtjckt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2flivuzxx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2rcermnna.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2fnmekeuk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2aaxagftf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfyhsdac.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2nkxmiaiw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2bovzbumv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2kiinzlnv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ndqjlwgn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fdjvswvs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yvosqdqo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2hblkezpn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2aerjmdle.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2vkvimijt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2kcsczjfm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2sgjstkun.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2afqqnlzd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2sojweema.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2wrwldwvh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2llbtlris.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jnfrufhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xqtaarru.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2axxdobbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zruxysum.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2arvacvvc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qkoiaqgu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2jbnqkuvl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2acitlwkw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2dfddnwua.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kkngkult.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2azgxsusj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xcsqeljn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dyyjgtfg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2lkmjutba.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fnmrieuw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hrgsqxzq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2egryswxl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2zrwgelvu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ybbnrfub.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tdgqnbbh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2hboldnrc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2skjufagq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gjhbvxxf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2vfovkxqs.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2kyglgwkv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2trnpebbv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2rctifqpf.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tosbgzzl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zgeuznoz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wsvueohp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qzeqzwam.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2yqfwfqsw.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2uxtmdhbg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2huiagpam.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2utxqgzkd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ifccbkei.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2xskbbflv.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2twagdndm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pdxbywpb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2lvhbukzl.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2sjthcity.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2dvzzeppo.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ktogslig.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2kxysbcar.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xadcionf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2kjlqxjoe.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2swcnbsqj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2jjctxbdv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2fishcpht.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ywslyrxj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2uzjhfvks.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ilgtikso.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2urylbmzz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2dziafflx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2aqypuabw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2bwcvmizt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nywftzte.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2sfcdzpjw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2jftizqcd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2zunklydn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2dusfsxnz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ubfxgoxg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2umvqyfdj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ntidbxri.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qyhgznuj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dlzkwhzb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ascxbfsh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2hflprafj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2rlmzdfxa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2qxzsrkmu.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2twcsmzfh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2xrwespsw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2esfefwao.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2jfwrhngh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ignwhopc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2tzlglewt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dyfjzmwj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2nxccpovb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ligxmkha.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2qeavsbkg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lrancwxi.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jsdwjffj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2pcvtpfil.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2nezffomd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zaovjimi.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xgvuofhd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2pcsaedge.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wudmmwdo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zqyinyei.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2xkmwejcj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2chuvdhyq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2vpyglxnp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2lrfmmlpk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2bqdnuhps.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2quiwqsjh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2jrtvkcxq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2skaixwcy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2yesqxgsr.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2pejzcgvk.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2hujidciq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wmtyrqqy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtzxwnks.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kicmjwdg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2vnitqpjs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuamiimi.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jcqyhknv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jqprnqkj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fcadrbkm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2rckoacxj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fojtjshi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xbutvqmo.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2cwtgdocb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2qrjrwrry.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fwtybohf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uncrgjiv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2xcebfamm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fggxyhpv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bearwctq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kvzwphnd.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2yjmhjeip.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ffogzhaa.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2zxozcgni.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qikvgxsc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2zfalxxxs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2gxjnqwqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcotbgmd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wwkayfeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tnuizawo.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2wqclmcyi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hdrkfssf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2dgcutoec.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2loatiunb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ubeuvfyy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2cbqlfyka.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2szarsdkq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2yfgbcvpm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2zrlyetvy.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2trcyzcph.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2nvqrkfpu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2wwhabwsn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2duwpnkru.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2zlmruqdg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ysewwrjd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2thcvrywh.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2bbexxkip.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2zfjcheco.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2dawugsqh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ugpcrahq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ljliphpo.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jxgbvfvg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jzwbbiko.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2czhymjzh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2njkikobb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2oigdcgcb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2nrbohqmo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2xbowwvwn.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2bqmabbbf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2urjlojpp.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2fcdqiniu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2zgeueeqx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2gizrqifp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2gsxyvzfu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2uuzamhvw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qhoqlmou.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ddyauecb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2noabczkv.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2zkhilxms.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2eekacmsp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2eqcxkngy.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2yesequtv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2zogylrmr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ijtedxzp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2slcfcjqt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2aggynmmu.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2okxrfxlz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2trhklsjw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ulfdszxe.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2pfbmkusa.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2fedaedrp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ohrdmeuz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2gedyontx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2tzanomjj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2wdjsigls.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2bzdmdmnx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2hsujvafn.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2hejudrms.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2jtbuyzrv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jtkokuzt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2hbragfew.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2naqhfbgt.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dgrvejwp.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2nymneyhg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2xfkvgldq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2jhxvqznk.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2rhczkzlu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2dyczjlex.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2mbexycrz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2mecbvtwa.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gkcqyqfy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2nkgrvmoz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2pstyatkh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2cwivydkh.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2sjgxbdue.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2aqixdsdp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2etaeehzr.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2gdinbpwz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2unduclru.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nxheiimc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2kxwmdmxv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2cjqjmafw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2apuqvzos.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ocbjnrsv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2elbbbyac.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ospuilow.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2nxvtjsed.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2brzklhta.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2jwacytnl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2osqfmjhd.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2aehlwtrh.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2fvfkrrrm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2msqlqooa.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2novnhken.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2axhigmtd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2akkjqrfx.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2himsjebw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2wxximzfh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2exzjgtdv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lztnttno.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2nwjwnqxw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ptwhnoah.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2csacgmsn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2lqwvnqhv.html


<!-- 参考信息 -->