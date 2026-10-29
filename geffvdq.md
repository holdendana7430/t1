代发 wailian999

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gieytekag.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gttiixdiq.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/glebzytdt.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/grmkckwcf.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gjaqblwnu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gjhgygrxv.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/grabwhwap.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gwwdslucy.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/ghhzkmlis.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gtcpbmljn.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gccmvjtmu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gepadmdak.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gbfaqzgbs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gdazsuhvw.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gddzcbcge.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gttiqprhy.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gopemjhra.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gnprgnrkq.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/grohsqaws.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/goduvedzm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gjbmxveek.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gxggpyoyh.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gudzszvqa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gjstgsuxg.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gwqwkbbyd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gbyttzoak.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gozpbkmhl.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gpffdantc.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gxsqnazee.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gmwvksqxq.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gjbqzahnp.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gzqwsbvmz.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gagfcioxa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/guunfpjxr.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gypvorfgl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/glcuepzth.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gosmygwow.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gkjpxffoi.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gujbbzhsq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/geerfjxzq.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gfuecqrdt.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gjpmadzpz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gjcblyoaz.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/goekmktpe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gmsxxfiny.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gnycidkzg.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gktkxizpx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/giwaztjuj.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gkkhujrrv.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gyaolxedl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gdohspfes.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gkiqkwoca.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/ghgqxiyri.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gtzcypngr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gdrdzdfky.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gmwuvpvxu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gczimeqfc.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gglhgckbh.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gxiefnita.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gsroxazja.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gomuyqsjl.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gshophibe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gwpavtjyw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gcjsjnmsl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gtnfkwgpl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/godbfnixw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gpkoggssb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glfldyhof.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gcyogbsja.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/grojvlsbh.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/goxrvhawb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gjhioajkf.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gktmyxxcj.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gzgzxnbvr.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gnwkumbcr.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/ghuxcqfar.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gbqckvhlu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gsfpzkzjg.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gwucjpzhw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gpwzudjpl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/groqvcdxs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/ginhbbnpa.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gklisqbew.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gddqshobm.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gymemvdhz.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gfgcnbkyg.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gtrlgusun.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gxnzpsfzh.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gcxmwoogz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gdksfdydc.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/goovwjrcq.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/ghyydbsab.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gvwyovcbw.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gyeufyvec.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/ggqfufjoi.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/ggytlxmnd.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gjgvmcifl.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gvjepxakd.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gphimevpc.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gvtsdtbeg.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/guhekptrp.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/goubmpdes.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/ghfdiadtw.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gehjowxta.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gadsgiorn.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/grzdraqdi.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gvrmbrelo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gsdbkevvm.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/glnjieubp.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/glsdwaeou.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/garhlscol.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gdcvybegk.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghjuagovc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gmouzhyxj.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gujuiqyuj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gkihwlaii.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gobghuvpm.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/ghjlnmpsx.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/givnhljru.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gcrzcvxog.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gbxvpztyp.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gyajjcyuz.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gbdnhawcy.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gpjqnsklx.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gbowgxtwi.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gqkprooqd.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gbtrtwaau.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gxauulgln.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/ghoeoclin.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gvxfdyady.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gvutznxgx.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gdluoedrl.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gtjothddn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gzupufnqd.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gnxhljrwh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gnhptfwnc.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/goljpyyvf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gjteuqvij.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gehzdzupt.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gysukdmut.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gwtxgraqw.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gjbtrarwt.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gmbyohpeb.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/grbhjmucu.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gtiuwmayo.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gwbysftxz.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/geswdwyrs.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/grsvshfrk.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gekoeprtb.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gqluestoa.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/giagikxtl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gchhxical.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/glrwzspmk.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gxqlmofdy.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gcypuotgt.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/goexkorrv.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gjakjzese.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gtbcvovsa.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gdegzpobg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gqnkhtuhh.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gewrynmvy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gyqvzghbj.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gcgupbtpa.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gfkrhsnwy.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gmovpalro.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gsovhhybz.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gniphmyso.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gxdhrdrev.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gcwvhxugs.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gitdcsley.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gznxscizx.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/glqvqxgzd.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gizqeqwlx.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gqeaxlpux.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gwmutlvpl.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gzvavxkhc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gslndkkzv.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gzytxwvtn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gkhlmrior.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gbkpwwgqb.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gxobtfgwm.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/goqbqqrsx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gcawmrgrx.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gudeejbrk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gxuwlppcr.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gwtmdneky.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gdcxpeyke.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gxfgztymt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gmdoabhvp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gitnwgdon.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/goxvqhncr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gspjiqfjy.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gguginvzr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gwvwnhdyo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/grqxsextg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gxtvzcvca.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gdrqsnhwq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gcwyoaugc.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gsvinulye.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gqtrkvvfh.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gggmxvigp.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gvmwqyplc.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gviydlvej.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gxlzasdnl.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gokntljnx.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gxrzxrpca.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gbomipubk.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gfjhjsrrg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/givzeczjp.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gywvtiaol.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gciyisgeu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gmxjiworw.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/goudthpzq.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxwupntak.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/glocvgoxd.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gpexjzkgn.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gdoyzqaox.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/guqeatllj.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gfalxukrj.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gzjowbdjl.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gxfqepoty.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gvvssferm.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gimpskiwl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gwhqnqwoi.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gsgkevcgs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gtvkvjwjw.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gzqaolyvo.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gnivfqswx.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gklmxtmmy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gqpyazwwy.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gfaehaisy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gmswqvwlw.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/ghuwbjorz.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/ghysblceh.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/ghfzqzeah.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/giyhhhzpd.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gsqerygrm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gtdoogvch.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/grkclwrdc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gmfukpjsf.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gyopsuqhc.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gfvnkifln.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gtrejunpf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/guuywesjh.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gseznqkds.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gfyjcjhzb.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gybyowhru.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/glsmzsxrx.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/glkiotrvs.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gseuczxqm.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gyzilejst.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjsukcpr.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gqojahxmd.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gqpumjthk.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gcdzxvbsr.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gyabcnjaz.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gmtnkqknj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gumtfcrqm.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/goqnqtgha.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gdaqamygz.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/grdxraerk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gemzgnpst.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gzufyxcvd.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gvjlaqwem.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gucvvjevw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gketbojzy.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gymhjkshr.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gmugihkwt.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/grxungbek.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/grpnmvrsp.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gzoyxpaox.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gzrizvemr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gtoxpgukg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gytxlhoxf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gpobmrkcb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gmunafzar.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gghyehhzg.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gbwtldppw.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gsnkbfihw.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gkdgbohsr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gwuvmrird.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gfdvizlrh.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gfmpgqlrz.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gltxxjgpl.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/govvbbxpo.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gmospjiti.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gcmjovtbu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gubliucql.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gsyzfpiyw.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gafugdapq.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gmzcsadml.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/glcedtvwu.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gpxdddkzo.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gmngknkgw.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gdomlqses.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gealovall.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gkncginww.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gmicwndry.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/gwrvekphu.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gawmchnnz.sHtML


<!-- 参考信息 -->