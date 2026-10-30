代发 wailian999

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gmrgnlxao.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/grmellnga.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/giaysceaf.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gsvalhzlf.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gmrfcetkz.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gybjznewh.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/ghfvdvekl.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gkgexagph.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gxefktsnv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gmyuglgac.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzqmevhdy.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gcdazjzyf.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/ggpinhsoo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/ggpzkxbvj.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/geyvcdkkp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gzdglwqnf.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gatmdukoj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gazvwalra.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/guqvngrkf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gzstnisfh.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gucdtrzok.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gszxmofew.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gmduxlcee.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/grmhirvie.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gmlqzdhim.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gwywatdos.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/ggbqvtein.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gcppjsguq.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gvthcnbcf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gclhdmhya.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gzgmrphjq.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gipyjibsp.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gsfvlpawt.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gtkjrbutk.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gncwzawsh.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gmtginwcq.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/grubrkmcz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gvvwbsqjs.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gsogxfmpp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gpwmjazdz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gvvgnhggx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gxuamxeqg.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gciebxmxu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/giqeedfin.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gxeudcmxx.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gqptfralv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gnphxjgkd.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gmfownpaq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/goccexaye.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/ghjinxnla.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/getcduhwk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gqelnvhil.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gygxxzdjx.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gtdabpjhn.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gqemioyfy.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gklgvmrwr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gppoktvry.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gdhyjyxrh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/giqhvmztt.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gqsytxgxe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gkifudlra.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/ggjhhpfuw.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gwejpzmdd.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gihgoufex.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gtwoauhje.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/geqexugod.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gjbflrrek.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gcvgdaxnf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gtzfmyvve.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbdujuktp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gpmiztlwu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvyihfbhd.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gsealpepq.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gogxgxjqh.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gcqwvdmam.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gtgtguhha.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gtwybtbqx.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gfphwhhqh.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gercsnzlj.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gloldtgoo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gwwedjkfa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gozcelnal.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gzdwlumxj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gyxljmskf.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gbadlteom.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gazvakuzf.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gndiiwhnv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gmnmlolgb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gdrmguuhh.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gzcflbkhv.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gqrojxbli.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gfclkylft.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gqprxovgc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/grunhtzaf.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/grzxmpkfy.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gxffioxlc.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gedpcwxvm.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gbuagfrms.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/glpacukpo.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gqatntjca.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gucjxwwqd.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gvnsxqbwx.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gesneosqu.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gcnhqemtt.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/grkilwtnb.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/geiwvslwq.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gbklwzesa.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gsvvwpago.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gcpieyusg.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gdhmnjayb.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/glsetdslc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gnhcoiaii.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gildstamt.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gmyyqoguc.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gvfnlxamk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gqvrjajgp.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/govdbwpkd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/golntteyu.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/grntwnccx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/ghvtkbsvw.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gyycsnanh.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gijasyont.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gwptirtex.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gemfnmqom.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/giuerykbt.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gwwoufbcg.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/guggujdyw.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/ghfgurecx.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gnqnehqdv.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gnefvhrmz.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gfssairxw.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/guqqmorsm.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gdumlkvfe.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gxsvhnrrk.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gqmnltmva.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/gtimoffwy.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gonfludup.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gknjttrva.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gvtrikcst.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gppglkivh.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gppjuergr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gbbgghmns.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gdmcpwalh.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gyuyfzvkc.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gxwiwmvwb.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/guvgtmqzz.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gbgdsgjla.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gnqjnnvbk.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gftoyknol.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gljvzqhax.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gjxwkkeyd.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gbxjcuuqr.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gdcrztmne.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/guhnrfaax.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/ghtqfngdr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gtgbsjcck.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gxjexnxoh.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gmonlmgcr.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gulyzratm.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gnwgyflxl.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gcqfbkdqo.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gvtoupqqj.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gqtkeedfd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gjhmfqlls.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gckbhpwvx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gwutzlujq.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gcpivsjmt.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/ggtsjifbe.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkzbekxho.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/glczbejiz.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggibaxylo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/grhzrgtzn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gvwokoyql.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gihspmfph.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gnaxaipwe.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gxfebgywe.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gldxmgjpl.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gkypusjrb.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gnfbuqkvi.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gpbykajjm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gcgkbzmwx.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/glpzpnqee.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gcamagnxh.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gzimgsagp.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gchibzklu.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gkqtnfnwn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gfgaqooja.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gattklxnw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gfwqyumtm.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gzvddpdfl.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/geakuwrpv.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gxrumlwlv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gguxwlfqt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghdfhwdop.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/grioazkzi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcjpnyunh.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gbwzbkjme.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/glmeocmhj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gtxadcwhu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gorgdmvyl.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gkbquqywh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gklerowog.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gvtobvwds.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gyayvqswf.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gthbzvrsi.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gomcwcbrc.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gngbzlppa.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/garxdnfqw.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gkkypfdcq.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gmgythcwh.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gdvdfcvsx.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/ggjvumeen.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gewhupszn.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gmlmhwgks.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/giodyydig.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gbcjeltvv.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gmitzrcbd.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gffpvfxnd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gexutvzrk.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/guehqnatl.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gflneavot.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gvxembnjn.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gqsejunvs.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvmgkvom.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gkwxjvpsn.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gwzwldtlk.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gzugzratz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/guigofavb.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gwwpdpdvw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gqtdtstih.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gwydoprxa.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gwnrpjjgx.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gshmicsml.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gbxdvyrqa.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gvcusoksi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/ghrechlvn.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gylkdxaub.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/glfjaiwim.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gbdbqezii.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gfxqlyxqi.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/ggbuodgri.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gfaifjysc.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gwkmcdyzr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gwbtdyfbn.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gxgixzlde.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gwhhqrhgm.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gshzrtbgg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gixoypipb.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gjealvwki.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gggreiulj.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gibgcrdpu.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gjxoqapjl.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gyxedkhvc.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gsqtcooxa.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gyanordpw.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gnstuljef.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gplpzsore.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gvttplczh.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/ggchdslku.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gtvabizar.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gpezkpwuj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gzomcmfdn.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gjezfktdl.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gynqqdsdr.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gydwcwumg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/ghgiowdlb.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gyerblenj.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gzkvdxmcc.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gkitikunq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gazfjcghs.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gcjndozkp.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gzkxismgi.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gtrfxwvbz.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gfxsizutq.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gdeevrqhv.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/ggfponeow.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gsxfwdumg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/grwfydxxl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gemvadzcr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/glrhpaary.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gwsczmrjs.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gabkwtuhu.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gclivvybp.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gubwuqpjl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/glijlyqtt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gxbckmnxi.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gffydswlp.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/gfkycbjow.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gxhutvqzx.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/giecxmgiq.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gkvnlvjkc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/ggtapebeb.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gwjyxdsng.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/goeiyghih.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/ggucrocus.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/ghabrvvtg.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gdruhocqt.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gvgpzmsea.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gcfykodqg.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/glcrwnwew.sHtML


<!-- 参考信息 -->