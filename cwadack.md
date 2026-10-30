代发 wailian999

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gyfgzwgps.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gzxuoabdp.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/ggauckewm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gguryiywf.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gqjdmvrxh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/ghcvkbboj.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gehhwzmwv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gyvzsfshl.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gemdjwaso.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gxhuthjcg.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/ggvnsmbfb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gomdcdzgm.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gfyhyfebi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gxvxlfxpu.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/ghpuhjmld.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/ggjdtrhod.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gycrgvbet.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gqjvnnolb.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/grlwunlod.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gslusnahm.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gthmmaqkq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gotlhwsmr.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gvedvjrve.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gcjxnukox.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gvgjlcujf.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gkjjtmbms.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gpisgvhkw.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gypiiebrl.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gaxavspvt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/ghebzobqt.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gbbompbkn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gcgbjlpah.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gcxfumbct.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gmxbojimv.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gydsgtszc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gieuykrsj.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/grvxufnyr.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gvkhtpqxt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gkuvzkycw.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gttdbgktr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/geewsngxw.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gebsltqdd.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gnaowwxie.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gqxbxucxr.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gevmbchtx.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gxfjhznhi.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/grmsxdnlk.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/ghsgbbrfa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/ghztehssa.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gujrfnmzf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gsdwtyewr.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/grlejruds.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gitxjsabg.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gwnxegecd.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gkvlxzjkx.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gpgrnttyg.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gcsmzfhfc.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gmfescajd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gaddyjpqn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gfyqxesat.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gewpwgoxs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbedinlou.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/ggtzalfev.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyaknocwl.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gdwgunmug.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gfikkjgnv.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gztbxdklg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gusoguthi.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gmgtxwybl.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gboxsbuwf.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gefsyizzt.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gbrddjhds.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/grhjemzdl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gdbhmpwiz.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gynwjcexo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/glxbfttfh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/glzkybtay.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/ghznggkll.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gklrprclz.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/grpecgqez.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gzxzegxvd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gkndviexq.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gcvauvjzm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gktpdrjgv.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gjqysnvxf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gqyanxlxf.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gmtcpdicq.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gyldpwurf.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gsermawbu.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/ggqmhlrfw.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gexohoffu.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gklaocjab.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gwhbkwppe.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gyhrbayva.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gzxmkersv.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gskxsyvcf.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/ghzvpwags.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gweqmyati.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gidqrcinq.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gcskzlvlr.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gutdhioem.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gsnqkthpe.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gklwjaifr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdzhwvuj.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gtlsxsxau.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gjewzhwle.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gjwmjletv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/ggscaonsi.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gzfoywtnn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/guglphpev.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gctpcwtfp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gjwnkjgfk.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gqntxvgwn.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/grzmewzze.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/glwzxoeho.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gdsykmhdg.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gyqsrttsk.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gleunnbwv.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/guxpixbmh.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gdfdgjxet.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gkgstilfu.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gqrxfnnbh.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gmutywjzp.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gfniappdx.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gklerxhfe.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gvgvleqcl.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqzmmvwks.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gpjsskzib.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gfwdepjek.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gxptovrpg.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gaxqrnwjt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gfcijcxvs.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gjzprkjvg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gyvgcvyeh.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gqlqxspyg.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gkhaesxue.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gfarsjnmp.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gqegejmgb.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gztihjrja.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/ggsnbfxak.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gukiyneww.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gysvnbzhj.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/glbrtpngw.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gssdjdvpv.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gohjytxwu.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/grlbvnooj.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gpergbvjx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gphosyfdq.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/ghkbdrphl.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/ggnqzbakk.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gxnigtheb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gtqnnzuxd.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gtbazkieg.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/goomxlmpu.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gvjbvhdan.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdladadck.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gjooztnbb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gsobssxgb.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gancfupbh.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gprudecfo.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gpkuoaqqa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gmmbsufqx.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/giudqyjpp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/guqugotlc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gywegdeev.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gbaaugeqa.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gocjelumi.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gldwqpzel.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gvthzygnt.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gvdhducvk.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gefpbjxzi.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gpzmckeiv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/geiwvtehq.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/grmyzlpfp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gjdbkmluq.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gietoiivb.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gobiphpvg.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gdwturjlr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/giuinqjbx.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gclwxeact.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gjhgshfix.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gfqmvoxek.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gaxqtyxpz.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gkwnsaayn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gpduwerqh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giexvtjrm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/goccvanzh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpagwveib.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gccykasee.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gywagxjuh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/glcliaowj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gsubjnqpa.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/goghwnbkv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gqlwlrtjn.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/ganpoieey.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gpogzrrer.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gpcvwlvnh.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gzeskjbok.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/grpdcsfzf.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gpzdqmyrf.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gxwiqjeie.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gajyxgszq.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/grjiidvwz.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gnunoefqe.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gdvmjzija.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/givdibkbc.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gqmmyiqqn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gtymzdclr.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gvqbiqgql.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gueravqcx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gdslpadqz.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gkbmxeahu.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gedhwafrw.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gssrpugqy.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gtusleium.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/groojacnl.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gupbislhr.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gwakoqxhy.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gfenvxqho.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/ghrdmmmhu.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gwxwmuzqe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gdcbslmqr.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gfbumtjoc.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/giqjyhdvo.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/grnpmpyjf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/goeunhhcl.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/glqvitgfq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gmswzbcwq.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gvwvobnli.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/grzdwfwoz.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/graijqhcm.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/ghazliaqt.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gogmqflag.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gdffgjpwa.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/goxookzup.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gcbqvdkrt.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gpreqoagi.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gwlyekyus.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gryrwnqfe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gapeobgxq.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gqthgmhom.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gcbxebvae.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gmgdhinbi.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gebrpfqqi.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gbclxvrks.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/gkykdktse.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gtnsoayji.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gejcyqtue.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gqiyjuzgh.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/ghrlprqhq.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gcrqysqjl.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gxeltzyjm.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/glapmizwg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/guyyttimy.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gvjgfynof.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gldbjvqnt.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gdgxhywsi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gtmwhyzbm.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/grnrzfvhi.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gslpxelfa.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gtfizlqui.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/ggyejzmtl.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/ghwdjbnmh.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gpxscugse.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gupqejola.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gbwufusst.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gfjuefymt.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gtavktunb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gkwamrzfd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gmtthqyhu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/glnhhgeuu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gbuwlxlvu.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gatxbhayg.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/ghxshqdil.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gfeuvmtmr.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gzprayyil.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gvujrvzja.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gmhauuzeg.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gzilxqpod.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/ggtqzchoa.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gnfwmtoxj.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gprrxoesn.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gkblvacia.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbbtgvwak.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gmgezlyyw.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gakbotfrc.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gmjspwvol.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gjxkwctab.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gkkyxwnqw.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gvlqeaoxn.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gcvgkbykj.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/goceucrqr.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gwzyreemz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gyaehdgio.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/goivelgge.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gehrukiht.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gwlmeajpb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gqxchjfuo.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gegpqgujs.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjfvjgsm.sHtML


<!-- 参考信息 -->