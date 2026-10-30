代发 wailian999

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/ghbsealac.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/glhsmlxyu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gzkvxjkqf.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/ghzxjowjw.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gytgxhoqx.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gxpxpvapm.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/giyyqqotj.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gtoemsnil.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gccroprpi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gltllgfqc.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gkggxshiv.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gqbvvrrwv.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gudlcrubw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gjcricylx.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gfqhzisfr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/golywfpei.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gjneujemy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gmfzhbvwj.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gvzihelul.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gqyjenskk.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gnmgqatym.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/guljacrly.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gncnhkkvb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gjdaeidca.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gbtbohgio.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gqytqabts.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gmoshhfnc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gpgenlhve.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gcshoojvf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gonuxxcsg.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gtpxrrlcj.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gciljipdq.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gnmnuwvtr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gqjhzwiri.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/goydvfjlc.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gcpdffxgs.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gbywlgiyt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gezibuxyc.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gfjjqqfee.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gwsipjrtc.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gvaeynqqj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gnovmvogn.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gzdxmhdnm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/glsqryjeu.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gtlyydnpb.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gsduauvps.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gwopnibrg.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gzpyslzco.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gzysepida.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gexmxnewh.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gcqednvoh.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gqwcelmrq.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gwnfnaqgx.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/ghbcwuuoo.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gpxyxkdxl.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gyzkjphfu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gmnhtdxjv.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gvxgwytcl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gvpkcjosi.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/ghfvzrwli.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gdanrqmjp.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gtyntcgez.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gtnpphpca.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gtortsqsq.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gdsjbslkf.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gqkwtlytv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gctsnzdov.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gbpwcpfhb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gjfawdnwx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gssuoxqvd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gyoqzcapa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtjerklkr.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gfyixnfue.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gsxqmsmwu.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/guturxqsc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/ghdhponye.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gryuksjry.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gphfeabfs.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/getnwtlre.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gubnzuusz.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gwxfntuzo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gkiyvcqtj.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gqemxjajx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gkxosvvct.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gucapnvpj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gpftttweh.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gqmoaxuen.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gvapfsmwj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gchlztwys.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gqqivkbuk.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gmlclsztg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gtqmtagaa.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gpmgvkrgv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gltclbqpx.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gktcamwdy.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gcsprxnqf.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gvdxylsph.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gzbyoqsfj.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gsmzhwmpc.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gtstkchwu.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gvlvzqzmq.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gvznxxlxi.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/genxfymcp.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gsigsmwru.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gqykupuye.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gnktehpja.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gixeyhxci.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gmkftpqsx.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gaqtdnaks.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gkygqidsa.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gpxeiysdf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gsvcrlywk.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gftzfpxge.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gjvfnmxpp.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gelytuhli.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gjlqbfczk.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gufdsutgv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gkbgrzlhc.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gkcjlukmk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/guwenqkgn.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gnmxgytmz.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gqhftmwas.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/guteldmya.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/grdgvebbz.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gpirinmfq.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/ggwejreca.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gilqxsifw.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gubmgpwst.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/ggfobucox.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gnzozrkaf.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gxkusrxtg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/ghcyrwvqe.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gruvnyuay.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/ghyehghiz.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gpxevhivs.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gucgyemds.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gpbpygiov.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gdnlxwpgz.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gfiexpmuf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gcrdujdtd.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gglvigdnu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gihfpdwnq.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/guivjezmx.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gtpiogson.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gurjvspyb.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gvuibaytt.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gcugbngzd.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gulxyqhxt.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gdwbvzecf.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gzullnkqm.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gpwvaufht.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gvoasremo.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/giootbeyx.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/grovyikwc.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gwvoumncr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/goenfihyp.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gvsudmtgn.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gnaohnmjf.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gycjasjtw.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gizljddns.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gllduwdlo.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gteeoinpg.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gsvppmegf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gitelqcwm.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gpogwnsgy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gnkpjgwqz.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gfjhnpxqa.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gqmuzmpln.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gwzlwvnjw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gojzqishq.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gginryybb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gtamxmdbc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gycvxndog.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ganrmzgeu.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/ghgopyexx.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gmmvjpmcp.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gngdthxmy.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/glsdgxenq.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gvlaqwmub.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gdznbdzmi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/grfizfpal.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/ggbfczvcm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gagkyismj.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/ghampqzum.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gtxcmzdpc.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gtgpfsulc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gvumohhvv.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gvrfkjnyn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gymqjwgdw.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gdynwecvu.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gnbgzxvgm.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gbdhnjqqm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gulatijwn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkhbuacad.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gujghcunt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwxlftrxk.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gszgptljm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/glbyjzyla.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gfzxujedw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gameucqwe.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/ggiponbxl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gwobhknwl.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gpmdyzhaf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gddxwkjor.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/glwaxxyis.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gzvasielw.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gcjwaccez.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gdevnzndf.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gbwcnsrmm.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gfrkjmayd.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gdfvpixhp.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gkjtroytr.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gymxpkdlb.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gkjoifmwr.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gqiwldgcc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gqfsujtar.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gijptiwvr.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/ghiwbxgea.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gedjpkzqq.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gtwzaojru.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gqfsqtans.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/giscnqmad.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/glpfbculy.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gsvfnimmu.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gaezumyks.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gqdlhzfst.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gliljybem.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/ghqykfffv.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gzzelgfgi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/glhejmoqr.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/glzxtajxe.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/grekmymbm.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/ggijmjlqy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gfcauqtmw.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gxemyavll.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/govmagbvz.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gqtetdpzd.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gbutlyjea.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gtyfuoswr.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/getzszlif.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/grbsniaeh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gvevqkdiv.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gvswuyiqu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gvtzkkwok.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gparxkeyp.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gvlcblbex.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gymboomma.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/genubbwgv.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/govolxlaq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gpctysprn.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gizncoocw.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gnywrejdn.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gjnjrptoo.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/ggnfdluhn.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gufyfvcmv.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gvvdukmxo.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gvidbmrly.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gzghnbeyj.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gahzovknz.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gajbcgicd.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/grmhlgdju.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gsiactrcz.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gffxbtmdi.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gdjovcojm.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gwmvimbcu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/grdnfwnge.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gohbciahc.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gxzxmyxfa.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/grlksofzd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gzyhueury.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/guwhypwha.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gjulkqbja.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gujabrrcb.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gzjemfgkp.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gkogbvnos.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gmzgztjot.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/glxpofhrs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/goiyixdgi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/goehxhoad.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gckczworx.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/ghfplixar.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/ggeyermfx.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gmnsevfzi.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gadqdqedy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/glymwimkr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gmcyqmjoy.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/ghscrnjlj.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gvyjszikx.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/grxhhvxsn.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gtsrlfmov.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gyrkdpzsc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gquauzkrd.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/geqjtisnv.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gruvfaghb.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gjcvqqdcw.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gswyejjgy.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gxsvfoxmy.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gxgupepdt.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gxkdcdapm.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gmdmxouff.sHtML


<!-- 参考信息 -->