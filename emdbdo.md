代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3kgzbetan.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3xiarxbml.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ccfahagf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3kaktiuzk.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3qssfgler.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3sypjpmqp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3jwyjmnzi.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3dqpcmhsb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3suzkzwmc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qjvjbnlp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3gkzqqfma.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nxsshtfz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3kethnlwj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vilkujon.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3lzngcrjc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3augwtyqs.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ockqxepd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ispeivmj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3emjamvug.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rqvibezv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ljloieyt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qkqmkhyu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jdbnhcxv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rcfhyxni.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3uzgqpmtp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zimjhhop.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ndvwwxsd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dgvhbfhi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ylfracwr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3tonshszc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3pjiooebb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3wfgwgnep.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ifnwftxq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ggdfdpaf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3kpedkmix.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xmnqqijr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ykbhnqtm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wwdduyzg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3kiqzlosk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3eiordqch.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3tnumaqve.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3xpjvumyp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3efetqlad.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ibulwfjt.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ztggozud.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfoqfwez.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3iftsjjje.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3gwbcvvnr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fcovxjgg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3nudanpwn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3hwanhxrl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3coccpcau.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dificnhp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3kupaalha.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ntcscdpm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3istgeifw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3nmaskxdb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3tjkfxuse.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3yuuvrfyl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3tlnseacp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ymcqdbbm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3gfjvbdqr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3weozcsld.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3xgqwjdrr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3txeebsxt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3astnalvz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ezzpaobs.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3yplxxpqk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3rjjfcbnm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3uephfwwj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3kjbeqqob.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3epnokknz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bjmgdfbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nnlrwaje.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3mgyyjqia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ardjgwmq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dvkszhfk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fgpiobsg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3knncxlof.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3oowhrswd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3xsgtfisr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3essaiqrr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3crtocbtg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3vwfbktuh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3flawupdg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3sfygeucy.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3orjushjl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kkvtpwpn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mnwfyuww.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wwgexiih.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3cfoawlfc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kebdevhv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3flkdtxno.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3rbtslmha.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3jquggtjp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3pestwias.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3jpnuhxmv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ffmooexs.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ptlfaxdg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ryvfpwga.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3limfimkn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wdrrhojz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3okazqbux.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ydxtiyzh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3qvhdfbnc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nkfynyvt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jhrvacsd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ouoruskp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3uqugxyvw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3xgdgjgii.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sjbdjtvn.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xsblmifs.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3owgcsalo.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3brhdfita.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3lnqkijre.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3epcnubzu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oorxxtpz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3cyrubyqv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3qunltroc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ecmqoyrt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3aodilabt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xaulwagz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qergduyv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hmdfzmwh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3yrarukpa.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3hqvhcuky.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3dsmssowu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3nxtbarxs.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jzxguvbn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3dmhumlcz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3lpffcqia.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3vfppymcc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3apsvuelr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3kxkrcofh.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ibnbbqqq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ispcmeyq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cmfuucog.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pjeifbjg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3iwefsbob.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3vpktcqgu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pyjuoman.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3rpejxflf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3fmdkjdmu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3efrqwpoc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vbfkriqx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3iywwgfup.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pvhvsigp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3qpfsovtu.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kptatgbj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3kjfbdetn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3nkyyhrlw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3zscxkjlr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fguxukxq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3klrrpiyw.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3vqbgnioh.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3fwtqirmg.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3krqnmwzc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3myicqwjr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vvmxukso.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rdnjkilj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kuwcxvlh.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3fnmxjtsk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3fborhuhn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3awcfrwmh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3stwtazuw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3exdzbbes.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3vtirwthv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3fgwbnvjx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3itzmqavo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtckergt.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3kkaeryyu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3knswnouz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xlvgkwke.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cysysmpu.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gfrmmtyt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3mwimuucb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3phyhumkv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3flaqymad.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xvibvuos.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3oovujwds.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vsxfyefz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jibnbxju.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3inqzgpcd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nfwgzdqw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3pfmegqcd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fljnaukl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ecmrfnjj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3qeaqlcsa.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3amkommco.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gwurrjgt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3bisruupp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3iifcueac.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qvqetunx.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3qwnfhuhy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tjfyvqte.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3yudfacpk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3tqejfaly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zohjhkqp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3bpjleyva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfmffmcp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3jcdmxytq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3vczddzya.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3hnyqxmsf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3zascbgtd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3icywpfhj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3xvskkvbr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3avpvhinm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3dsvrvatb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ipscikhx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qveoxcnq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3pllpdecb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3wbeeybks.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ossecrbl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3wmbsbwbh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3oamvvgaz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3sxxhfoiq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3viccxtrj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3uulhbwrw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3aojzqdos.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3rcozuavt.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xzwmwbew.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3egwobnqt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3dqkcqdfx.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uvjutail.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3xiwivcxk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3xbsmlfil.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3rworkvec.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3znfzirbx.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3xclkszns.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3euzrropb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3avthkcrs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3vzvlojng.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3zmjqfokb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3umfayfxw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ojcxwymo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zmjjxtvr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3eqjczvgn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3agpxxxfx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3fkbomadd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3pizbmwts.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3yncxgeez.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3wwehsjol.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3znsikvey.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3rgnzdfml.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3bbzxllmb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3bpuoftib.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3pkqtylpc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hgfydzth.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3hoqpwsdc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3clwpaamj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3zyluoybm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3wovnvpvj.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3hxkeaxru.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3qkcrxqyb.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3sisqmrxb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3raeykxkz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vswesafg.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3mwuswdsa.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3tetarvzy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bkawvbhl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3nxtolkpr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ozgszaag.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3matmvecj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3yxuakpdg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3kqagcdzc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ixrzsxai.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3mqhotcqt.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3sukizhhw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3qoczxuvz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3osjvickb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3jtqogqsl.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3whqkibhi.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3efzhbbbl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3evjmxphj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ccfmuybv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3psypdnos.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3zjyehzac.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3kpvfphqq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3pidcbdef.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hppwrnoq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3syzihtvp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3jyjntklk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3yrdhpzzd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3frhbfshq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ekdmmdnd.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3pyulepuy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3iwjvnijb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3qqvviped.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ydxvjwiu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mpbwxcdv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3zurbqgjb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3eltooqne.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3qlwbgcog.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ackqpjdt.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3xduhokaz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pypzxnfi.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3llasolxo.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3wjngtpcy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3iduppokd.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxbidruw.html


<!-- 参考信息 -->