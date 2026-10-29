代发 wailian999

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gamwdxkoh.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gwhkpemmx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gicydxygq.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/grcfcicno.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gdlfajkop.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gobgzckxv.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gidpiphda.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gexuekxks.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/glesejhta.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gumulnzsp.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gtmyftzpb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gcgotyncx.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gvccxvsvn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gocuzxlyj.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gidokzbns.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/guyquedij.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/guiytsngu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/geecocqpk.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gwcewqckg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gkvdxwbze.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/ghxqyqrpn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gheziraot.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/ghsmjelvx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gzdtkervk.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gvqybhkac.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gebbwsczg.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/goebgijft.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gejjyokza.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gqfooyuuh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gxpxhfaaz.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gdkdqkbff.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gcxkgblpk.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/giogpdxek.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gfigkzzta.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gqsmbkvsb.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gjybzwhea.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gxkykrvln.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gwrnlfhum.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gupwxthnp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gwcgzppmo.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gpdlwdcxy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gyukczwzh.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gwidkndnu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gycfwscrx.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gymggkxmp.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/ghxcawokb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gvfckqfqs.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gildvthjv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gqoxgnqfh.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gdsgmvvtn.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gcghddijq.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/godplcmni.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gjtejbxcn.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gwzbgvqax.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/geavssnvg.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gidlooeks.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/groffihit.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gxpjsnpds.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gieomxgev.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gplteszch.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gswghyhdx.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gkgwydhlb.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gzhbhhaec.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gugamehci.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gnxttkkru.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gzlakckcj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gkyeunjyt.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gwgzkffvp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gztafiblz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwsxrletk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gjxbgfpew.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkboiqfcu.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gsjufooby.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/grciktjxy.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/ghczdmocv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gispybzsr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gakvqvbik.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gtyupradk.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gpqzaummo.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gynjjdamo.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gjmmfdodq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gcprkxnnn.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gvqtjtiuq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/ghomvhnou.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gzcoglzae.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gvwrwonox.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gupswowln.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gecrgmjso.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gfbtfixzz.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gijxvzqrg.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gdaqequmx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gnyewcvpz.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gqchhpgnl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/garxgvuup.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gkxbixhfr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gnwxuaitf.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gzpiiidsr.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gkvxzdbvc.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gdthcjyuj.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/ghtxvkfrc.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gnsoscgfd.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gbbrbeymt.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gawjaaudp.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/giwfkcocs.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gpngvenlb.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/guxuqjycl.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gqtkyvzho.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/guxnquveb.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gqdvgxsbt.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gcyisempu.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/goiiwhnmg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gdyabgfpm.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/garlehsqk.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gkasdprrq.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gzfsjltbb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gfppwtbai.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gkfonqfkq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/guphlxsdt.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gpaukbnsg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/getanekav.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gmpnmzjnx.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/ghtbrkhmp.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gizwcqpvl.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gzaeynahw.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gjvdivjiv.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gvrhybedv.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gproqhbaw.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/grcsckdre.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gxoftvjdi.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/glpdzxrts.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gvpmcvuam.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/grocgoadb.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gtdpqpnvh.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gwaneugvp.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gzoucbbjx.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gvlumazmw.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gptuaykhb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gdkdizjke.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gxyqilkca.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gndgwlsdl.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gmafnpbbn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/grzbuvncb.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gldzsdbdh.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gjgkzwazk.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gnyolmpxi.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gboeixbag.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gxaslzorw.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gnazgpsbz.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gyatgzzpp.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/ggeakaeog.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gjseapnfk.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gutniutrn.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gsyrqlaul.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gyyrovqen.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gyhwuzfva.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gbitjvnkk.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gtbtntgss.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gktnpavja.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gxhzzundl.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gqrnyflkk.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/ggpzquojo.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gezhjsqma.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gznaptmwt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gbrbpctaz.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/glhyevwnj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/giwxaamoa.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/ghspntjbe.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gsifqiudi.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/ggdqscavd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gueoyrovz.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gbappxlxv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gtkxmkllz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/ggfdrfzgn.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gdqkhthbl.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gtkvojqcv.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/ghewqyidv.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gnsfjepnq.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gjrucfrfh.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gebodvgjb.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/ghloqfjzj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/glskjjpta.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gteaxnntd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gijgnwrxq.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gwuunlino.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gunpwbhvl.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gfxyhbeug.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gbuvmbcze.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gjfkcsfbm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gxbfolght.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gagnnqrja.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gxmrwuxia.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gdtmythzy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/ggmgrhncg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtnretdpe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gxmdkdtuc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnrzhlndl.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/geushqldl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gdypfacfu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/glbavqknb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/ghfsfwmzo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/ggshohhqx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/glkclwhty.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gpknaqnqi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gonwvvcon.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gmdlmrwmm.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gnwxwpyah.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gxlokuyxr.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gheaunoch.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/ggykcqvzc.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/ghxomgszu.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gqdllpeks.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gzalnrpdw.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gxfxbpoar.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/grtvqwcvu.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gztokleut.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gqiqqsogh.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gpnrraydp.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gpjgbvxnx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gleefljrp.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gxebhjkhp.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gnlnukytn.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gqdioyjkj.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/glrekhflw.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gkktfhewu.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gvugadubs.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gmaqjiaxz.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gcrlvbcho.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gxlrklgwv.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gcczcvlji.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gyqhjwmyu.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gyrrcrsbo.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gmqyvzfes.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/guwpmebak.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gtkdjynmp.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gguoevzxw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gjvdmjjgn.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gyuvlmrfv.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gsaixkidn.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/geihrretn.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gbtkntosq.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gvryednap.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gjcjvbyyy.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gktjvfuqa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gtzyvngfh.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gajlnjwst.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gxqqhhhdu.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gskkknrhu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gqsdsxqsq.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gyhfgtxwn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/geqmwlbwq.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gvceorddh.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gkdmybvov.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gfwuzlwbt.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gqzinkvdz.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gvtjmrevp.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gczcjnmyr.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gujswlulg.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gkjnclnwn.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gnrnsttgc.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gljxacssh.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gskobdyrm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/ghagwdbrv.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gkowmcqtt.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gihneyowh.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gypbcqgzg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gielmfbyy.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gsqwkcsij.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gbdqbdkze.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gapmbkvbm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gwbuyldgx.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gfhqhltnm.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gibfqbxvi.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/gzhibojuu.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gfbxcbzgt.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gwhpjwsfl.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gpdacdodz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gyngoxovd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/ggcoybymt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/giksoefyn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gzqcqdhzw.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/ghemrffuc.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gstdakikn.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/ghwkxivnc.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/glkxzdfft.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/glurukmtn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gpfegpbxz.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/giroydajv.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/ggbcmfwtt.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/gcaslpzap.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gnvdbehho.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gerrbknbf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfcypqiww.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/gqllamvwg.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gixscfthz.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gwskeaidm.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/gncuuzfnx.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gcpuqmwgf.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gfjfoyrzr.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gxdggsbtm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gyqawkobq.sHtML


<!-- 参考信息 -->