代发 wailian999

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gfghupzaa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gnthxumxs.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/grufmmmua.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gokuvrzrl.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gdjmrieyh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gyszvfdue.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gbwdknick.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gyvmzfgzf.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/guemcojsq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/ghpzeeofw.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/ghfewlvwx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gneerdooq.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gkxjxpkqq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gncqnmshs.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gjaoynbcn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gvletabfp.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gqzwtmcgh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gmgqlvlgd.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/geezgqvnw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gbwolnbha.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/geapetksq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/ghujxlmki.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gxulgdcwa.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gjuaquurg.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gvdyngqef.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/grvngfill.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/ggyggtywr.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gymdshbkw.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gvbwbcufm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gdpvniqlr.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gfvueqikz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/geipxkwzp.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gttrjbyfs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gskmbmfus.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gnwdvxxrs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gsyijsmsj.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/ghahivwsx.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gvtblplqw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gkcgqnsmf.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gqcchyysb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/ggfgmzgkh.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gwmffqaoj.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gednpygws.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gcfhnglbu.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gytogwnmz.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/geadtihbf.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gzznndivd.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gosicpxzd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gttfhojmz.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gmxefssee.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gohcunufl.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/ghlydhhpx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gjyflohxm.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/grmzmzxdz.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/goelcjqym.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gcybtsoky.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gbksxvmwh.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gqjslheia.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gzcjwflzz.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gzpvhsafm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gxywnyrho.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjgdbgsov.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gsypxzcvu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyehpyaqn.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gpltrweuq.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gzhjnroyk.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gbxraknqn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gpycaqddh.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gtimshmux.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gltywmshk.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/ghxllxfyk.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/groacvucb.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gfhcsbwfe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gkrczjuxa.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/ghgcthtog.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gtxljeoym.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/givjavdpl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gpshxcjjk.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gppuqkehp.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/goagdapnm.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gvctwrjgv.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gpccuvpns.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gigevgmac.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gzriacnqr.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gvnpobtph.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/glxdgrcwq.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gmnkugwom.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/godzspeue.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gnsocrwrr.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/glkmqehcl.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gqycjwjjn.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gttaxsptg.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gviiohkem.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gvsnuhuaf.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gzoeqndne.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gsccxiuie.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gziobxhyq.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gqsrewedt.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gvplmtrkv.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/grzvjwldq.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gnmirvevi.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/goqpvmmwx.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gycvmzvno.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gjebdxttb.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gtjikcvdf.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gqxrjybtw.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gvnnwwxhm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gwrwjulxx.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gnckeirmv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gwfsaoogc.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gokwhshdi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/ggplkxwdf.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gqraajkut.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/ghfkajupg.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gsbbudnes.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gshhxkoha.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gwpiwphud.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gxusakwys.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gehvxtukj.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gtbvfiktr.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/ggmkzcvtb.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gcrrkctzf.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gvojxshbi.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gbcnmnzgx.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gvxtobwai.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gdwwviffm.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gifpsqxfr.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gdfradzso.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gziwsqbgh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gwjedurpt.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gvkjdeyqj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gvokjidio.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gwhpcerav.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gutmzntxb.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gvmakfntt.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gpemtlpvn.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gvhzvgrhm.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gkephojsb.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gxfzhvnsv.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/geskigfpe.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gpgtwtpqp.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gbfgogqjq.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gdkngtufk.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gtvxhbutc.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/glqcjdslw.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gzkmviydv.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/guhjstune.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gbrlyzrbg.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/guwwuwiac.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gtqbxzudi.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/grtujbpxa.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gvqkjivev.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gdqlrdgee.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gsyxrsmbq.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/ggbhbghxd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gdromycdc.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gteafsjcd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gfdwkdrxc.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gozlxpyle.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gtcaqljbo.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gvhenkfkr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gvhjkmkpg.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gsoxmulpe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gpjbqudjq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gbxxqttie.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/gppznrsvx.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gepaldwem.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gwyqbeopu.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/ggrkkubvs.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gmmwdsbxq.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gkqkxpqoy.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gttmrusjo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gvaadhvxf.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/geuqzxgir.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gechbxbgp.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gaczcoywo.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gowdeixed.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gvlseryju.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/grzqhnqwt.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gpcqggynv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gvabaqqbo.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gubatqsek.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/glhlokyyg.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gcnljdbal.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gpzrzfjcu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gumrmptls.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gfmkggxha.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfrpyymjj.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gsjbbucor.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gvkbarvyy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gmusyjzso.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gegpwbnln.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gisjzeatk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/ggbvcwgmb.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gtmdiktmx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/ggpdcplis.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gkdufidgl.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gcobtygxe.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gtguhdyep.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gzpplekgv.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gmacbosvl.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gwmoxrvxz.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/glumoeqbc.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gnrpwykke.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gwhwlbrvv.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/grpigvnmb.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/grsdcqjzg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gdopcnafc.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gemdezopk.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gmhluacdb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gshzvjxgg.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gfmetjnds.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gubgzbvww.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/geqvpnlik.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gspojmtvf.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gkblrusbj.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gyodyikyd.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gkwinzxwk.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/grxpqngil.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gxxmywowe.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gyacujzjl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gbfqwbpan.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gfuxognaj.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gjlkyrili.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/glkzrngyw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gyherrkok.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gbivbopaw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/ghyvygtzq.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gxgtgazyo.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gngzcnqnv.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gbvbgawxh.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gqliktrai.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gqbencaje.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gwjufbfdd.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gkfclrape.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gktthbgto.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gwaksmhfn.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gghgoexor.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gtihfdylu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhzzflcu.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gzumttwzp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/ggipclmsa.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gusrcftgo.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gyiltatsw.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/ggjcxmgih.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gosgjhcfo.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gabfsfwic.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/ghqqqbrjr.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gpxxqnxpy.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gqglzldqq.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/ghhvgdwpz.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gpbhrygfu.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/ghabqysix.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gfpqpmkwv.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/glpyohlhr.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/ggigyqvns.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gtntcfwyp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gopbisvrh.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gyronrllw.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gllzwpedh.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gsbijhock.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/geuuazheo.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gvkvfoupd.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gmvcjtvql.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gughaygmy.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gyhqvagte.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gduhycykw.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gyinzuquq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gtwqyvgdy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gdnyryylm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gnqnhhplt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gbsmfjwrr.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gljobgyfh.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/grcuqsjwk.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gyaiipvcv.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gtevcyxsx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gukuweech.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gvihrhktu.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gsyovglwy.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gmquogppy.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gizdsfljn.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/gsendkpmm.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/graszdhmg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gbuwmcpjc.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gehzamted.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gfzwjejvh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gmbcxwdhy.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/giqwoezso.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gqbrojbgg.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gwlrfvxiy.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gjcoiscav.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gkdpjzhth.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gwhjanipf.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gmhbzhpit.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gjmjberhl.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gabpgvttw.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gtggqewrp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gwjeqsjfa.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/ggiqhtuvh.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/geijbkeaq.sHtML


<!-- 参考信息 -->