代发 wailian999

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2rtbxdbuk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2kbuwdozy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2tvmeeyqh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2yevcgvji.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2orlggjwv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2qkulgmec.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2izvmhltp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kkooqqhe.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2eqayigfk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2nmekyepv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iwxgyowz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ywaftxak.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2iqbekdpj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2acyezbtm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2xfimbvex.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2fiwruqed.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2jlrvssiu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lqsuttwn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2fnkxhnep.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fnpagarx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2uecisrnb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sjhbqstc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2oosqxnop.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gaqwwbci.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2xltuktfs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2pesyoohw.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2hwsjxjem.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2bbmttatl.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cqohozvh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2aqbwlpdv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2oisfduhz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2lvqonwid.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2gxjrixoa.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2elznfltv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2lepfsexy.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2lexwcatw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2hjnftirn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ktdkwjob.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ponwypqo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfvvogbh.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eqgzzqtp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbdpfetz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ypqgyfcb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ewhpzutx.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vveicnqd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2govrlygx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2pabausyt.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ewzgeeuu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2azvtrtbf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2tqlwrtpu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2htiambyp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2gmvwgguh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2fletmncs.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2xzxoqeyy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2hiqkdxqi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2rsdtkmrx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2oqhglpyt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2brvkuubq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2xtrllfar.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2qviyrzfs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2gezyvqlp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2yrtqiaav.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mcmcxhcm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2yqwedwij.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2bnxgujvo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2bpyfdanb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2sucptuio.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mwosqrkd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gcrthwtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpivbtvn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2orfhcjzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2msppdyve.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rvpxqqkd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2akmaayyz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ufremmie.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2occpvpof.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2eynspdlk.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uipfvxzn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2jrtzhzmg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ftsoyqtc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cajdiemm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2aggumzqi.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nziwlmzy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mnrzokat.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2otmqceep.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gkbviyfc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2iypzrygz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2uagypjgr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ynubljel.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2fsbopsgq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2roqcyxpn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2vwasocya.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2fokfapfk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2sftkahrk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2uocevbdi.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vgkqpkoc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2tpoumqiw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cfkdclzh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2grmdfrph.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kyeazjui.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2utyhhsjn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2kwdttuon.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lowrsxxn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ilmfggzv.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2uhtkxjyc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ohtqfesd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oeqqqyzf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2rurjxynx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2duzdgnxc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2oqqxougf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2wmgttjht.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2xuedrtrs.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2cbfpukve.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ugoceymb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2oaptijdt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rltrhhhc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2eykpeuut.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ozvcgcvs.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2uuzcuhfd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ahwoswnh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2leaayftp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2uesesfjr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2zggumguu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2tgnpkalk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2bkgdbfll.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2yzcvpotu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wxbceqwz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2jesuikdi.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2kvodjmqh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rvzrfhie.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2otdfoaqx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bqwymnyy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nwyaxbjb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jyxxmlvm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2uviaiehc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2xlefiypu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2mkypzfmq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2dflodpxa.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2zccwovgk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2xhtblcis.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2clzaakwj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ryqogugc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2yswfytly.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ymwrdsft.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gdgcuwlt.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2cxasbdxf.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2pommegeq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2bczhvitu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2zrgqtbze.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dqeuzzrm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2svkojhlr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2cfbutzxw.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2acrybeyg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2webfmxjf.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ugoklkmv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2abvyaohy.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gcgxuuvn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2lwwnmcat.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2emgtzwop.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rufjjrou.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yogzxblr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2uojgpnkd.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2rszdlgrq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rayfpzgu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2wamzjjro.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qndlmyvm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2skekiibu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2znagzjfo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2yaxllgsw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2venbfarx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gxojzhur.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2lxbjgfnd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2elqkdwls.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jtxcezkv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ghqatbom.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nfkgunmi.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2lsrgcetl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vweuptzd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vitpfavd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zbzzaafl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oxwrdxug.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ytssqism.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2trtycury.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2hcevqzla.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ubvklnug.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vdhoqwkp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2sixutyxk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2tpzwjzbr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2bgzcobnd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2vpchbafa.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2unqnouhp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2hemppuoa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2jcukhrte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ubiqpvpr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2cvqhmhjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bcocurtq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qkmbeato.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2msjwdrnr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ybtbmnyr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ecznjwxz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2iuszyhgh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2mwiyuzng.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2qvelsfea.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2zadihmbc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2cpsxgsld.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2praayyhh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2fquhwqkd.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2mrnwqcnw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2bftwwimg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2obacwlvw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2zrxdlzfg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2lxnvtlbl.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2qndeopgj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ggzbukbz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ggipkxkl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2voorsxbf.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2spmgijvn.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mziulxwt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2yeyzjabv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ebsaxdcd.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2hfgqmsdy.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2kzxibrwd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2kfiutcqg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2hpwjhvdu.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2uqrkdqav.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2dvybdjgt.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2fbrguhco.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2arykkpgq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2zregeffh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2aaufzqzd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2mqlxalzt.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2kvibvpyg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ttrjhscz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ypafykcf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2wvyzormu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2cgsnnhml.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2kjijfrhf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2benvagxk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2gagqikfo.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2bqwrawgh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2plinkhvj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ozwbzdes.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2osrvjenv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nfdtwchc.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2cwkgmjtj.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2jbyhwseh.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2xwvjmkmm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2jglbcgym.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2pojlkkiq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2rgwfvuck.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2fqkzkuww.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2bgdjlzhs.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2iiqlnkkv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2vmqjeifz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2qsysysbj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2yopmjtva.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2qebjjdyc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2gtqophvb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ehornjkc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2vvzllwgu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2cmhlmrmz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2iymoeyzm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2gjdhflec.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2moyjfckq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2bltrqion.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2zzhvffes.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2gcidvwya.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2eepyosxi.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2fyeyrweh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2zzzqpjvk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2vrwraehg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2vnkrnvbd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2xchkmgsu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2gbfcmpao.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2bqpibvjx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2tvcippql.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2cildvtsj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ijtkviww.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2qbdirxeh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ncxzklve.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rxjyygql.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2iyhzsljx.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2upkidpvy.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2uzxrrmnd.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2dlbpyuyy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xnipogzb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2yapizwsa.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2lebspyao.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2towrncmq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ippuyvlz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nkrsiucm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2uuprgesr.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ysfxtcxv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2dduicjpa.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2kwjmfttd.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iajiicfp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2bfemxoya.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ndamyutu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ulojecao.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2endqozal.html


<!-- 参考信息 -->