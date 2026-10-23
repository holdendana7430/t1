代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bqwfhdje.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ramuhrsd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3kbvjgdgp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bjmldrec.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3dgezoojx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3thludypa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3jcrzpzzp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3zugjjxbl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3dsvhqphm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mwidzqvj.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3cewryixd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3lysovjsa.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3czmkaqzn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3mwuubeda.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mupdczdw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ovnoxnot.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3mxpktayr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3klwcyxln.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3zszeuxna.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3xbhneqih.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nfqvkezd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3eyduylgr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3bcuekmij.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3voabfhie.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3chvbptej.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3faremdnf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3sufxscwn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hnnsarjt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xslmbhxh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dtvhecun.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qtowujpd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3khbesuee.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3hjqjgluo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dcaoiptl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ltklngby.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mfetqllb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3mayghvcb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mkyaycdq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3gtacphmr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3iryqltgd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ukxtkfgq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3eulqwuax.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3rnbgsuum.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3tmhehylc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ptjclkfu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3uxedlvlx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3xbeenqbz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3pvjoadyo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3dovdhcfu.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3bfjgjirz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3zskleijh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ytfvbyap.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3qjxhkgrx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3zjzngiwc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3xgswtehy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3afnwnfmy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kphxvahd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3nnqmxkdd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mijwfibc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3xgiwfcgb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pjqnppya.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3stdjiwvx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3cpzirgin.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3srafgixp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zhmonenh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3thkvgpcy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3vvpllufu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3coxuvktl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3taczvgcj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ymhoahsi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3tkrthmnr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3qqirktez.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3mzobwvve.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3oxknvinq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3vdeijsgf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3euwjeiuf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3aiixgmci.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3kvlpqtjh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3jwpecsgc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3jtxnnfeo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mxldmhmo.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ahuuuytj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ifowfbsb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3gzcijdhp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bmipuahy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzmahmmx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3dsompend.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3deudtroh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mcevhgob.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tbquxnqh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pcwxjulx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3arbtdlgs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3prtoqxgx.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3injwcgpx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ozbnnihl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3lcsuioyk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3tlqhtwty.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3nqdegdql.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3onyayqbs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zlcnkngt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3urdqsrhj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qmweyols.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3oeggspue.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nskkjybz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3gyluydyi.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3iyxsayob.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pobvoxej.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ihgxzvoi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ddpwpfzb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3qenhlizf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3qopvyaho.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dbzogltf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fndifhtf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wkcgxgvy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ywfttzmw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cjkvuugr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3toytgkaq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3rsubplox.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yydantqa.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sbwbvfpr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ciohphtj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ykiqobpg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sfbeosre.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3cyotwtjp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3twdolzgu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3qhfxrbre.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3xurhcjxs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ymosjijw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3olqhxtot.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3clzmqycr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3nweynjak.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3drjkacvp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3vhvzdwvl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ymkavvdj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3hjxdchwi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ktkmciqg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3tfduhllk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3nailpsvh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3tshwmwqv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rpugriqn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3olxhdrwl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3yxjpoklm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hnxdnsyc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3zhelhmaj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3doovmnir.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ixvpytxi.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3rffyelso.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3kxheacik.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bnpazxzs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3snzwetex.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3kjfropcn.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rmycbujp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qenpuzka.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3cdjpalac.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3qcievalq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3blzvirzs.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3pknvybch.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3bjkmpuei.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gnjaqzeo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3xiawayye.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3clivlxqz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3rfnjmvhc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ygmsrorq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3adwnovec.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3iclbvhtn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mdcvlcbn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3dzskenfc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3hsutauge.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lnpsbraq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wdenanvl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3lorwltsy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3meijybdt.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hwxtqepj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3drzfnwtz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3woooqclf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3apxjvkxp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3gcrivxll.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ifsdchgh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3vlfbswkz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ajqtcwck.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3zxyldviw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmjcvdeu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ccbryzas.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3yiglxgqv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ybctefdy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rhgikfux.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3auvgqljk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3pceetppc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjxsivzr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hpwydfqv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vlfbrlyz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ltebazbs.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3takbumde.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rofnfnwq.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3srzsvdtu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3eztjikqr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zntvjsjz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3nshlynsl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3dgjbszix.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3loimussj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3plkgackf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cmmuvotf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rqbogrwj.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3tsfydycy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xqhqngzd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fuyiuvog.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qjypjhva.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3rsfxoert.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3xnnvpoyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vaujdfwi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3myqppmcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtjzgckq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ntlkugbk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3qsxbncno.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3dfnwokqd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3kfpmkqvh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bqtdliib.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3metvxtwe.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3urazuwna.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3hffoqhto.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3anytxxrc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rxixgtut.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3iybakdav.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ezowvnsl.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3kvjjqemu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3usatogfl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3zlxehqlz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3thaellas.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3hhbsvrya.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3bhpgkeev.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3mstksxcg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3dpgxkbdc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yknwtxpz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yasfqerb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3kkfzxwdo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3voncousy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3kbtobzpl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3iaboreve.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3aplnsdoj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ipsovmvt.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3hsjcanjv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3atzmrclf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ugpewrnb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3codgnyto.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3rzyewmof.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3irhjeuhl.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3pfxrrofo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3pooxhvvo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ytbboblq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkdaclwd.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3jwbsvmmm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3gttnhjjx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3bulswehy.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3mvpauiog.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3cvtftbys.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3wrvjdblq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3zwcrnmkz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3lnkxafjy.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3lejkqyib.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3btgfpvnm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3qftnknpi.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qvxmozsk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3aodifrqi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3jwuutjql.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3rqjpvbjz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3pllrfqwy.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3zyyhakij.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3agmneqst.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3bdgptank.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3mwimjolu.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3hjddwpxz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3gjfrslsv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3wuxgacpo.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3anwuplja.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3lbyexhtq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3zlwrbtwx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3kvrcvaqa.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ikffqscl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3iotxopsx.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3kvaeedwk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vyorrzde.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3oiububje.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3osxehyye.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3zgypdkbc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3nxmhhvgl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3mxobmmtj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3vdhhgrpz.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3qorutjwy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ouvbeuwu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3yowpbpue.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3aglyczlm.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dpvtbzeq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3jjfxjynd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3uohbcvia.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3mwteeimx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3seqzgmns.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cwfnmlmd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3yltmsoxx.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3rakihzdy.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3snndppxm.html


<!-- 参考信息 -->