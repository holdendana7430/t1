代发 wailian999

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gpdrkghze.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gfodxjxfd.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gjxbnjevi.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/guaeabogb.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gabpjgzol.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gzrbbovik.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gtkwunpcq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gkyivrelo.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gojlkvvks.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gcgsdydfq.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gqtmzdtkz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gjhcyalhk.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gisdhjwrw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/grtcvtpzb.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/ggvrvptak.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gqcetlsru.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gyvkfntyr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gtbrmcqvu.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gbbaardfa.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gsgkzfuls.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gqahzfzjo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gwknlxfeb.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gkbmoruhz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gfyyzurzk.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gpechhoem.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gwgzjrbuz.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gnhzgfvjk.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gxsuqbpbw.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gasvevxhy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gvaumixgi.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gtykgyoba.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gdhhbkspo.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gltbxschj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/goyagytii.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gjozzjinr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gbmvxcqky.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/grioiujvx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/ghewsqfmt.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gddpasgqv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gcqmxgofr.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/ggsowzgou.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gdaqlotyu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/grplzdjkk.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gtvzebqle.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gltcnfojs.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gdohrwddv.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gqdtypxah.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gtkyomlhx.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gzvlohotf.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gngepwhkc.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gkgoavbnt.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gbayxgagf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gzfkniidv.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/ggcxmrztg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gexxjpuap.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gpqnpgtpf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gmhytkwqj.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gjdhmwrox.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gujmslnge.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gxqlnqwgo.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gjrbhjkex.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gjkwjgzmx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/ghfynzzva.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gcubuexfs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gdoiqfomv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbjdkwubf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gtywuaaav.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdvnypgab.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gvcsxlgod.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gsltergzq.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/graxcumgd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gutdptdxz.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gixwmmgsk.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gypxuhour.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gahcislnr.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/glwwftuvz.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gmgkpvbna.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/guymfeevj.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gciolnuvn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gjzyfijqq.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/ghdlqfxra.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/griljmzwh.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gbeloooyo.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gpdhjomms.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gnfrnipci.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gmnldqbbd.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gjsbaviaq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/grmysylux.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gevvweuhf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gemmtqzmv.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gsppnlsio.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gmqhovmhg.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/glynfuxsd.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gvgilrpkh.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gjlfpwrqr.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gibxrfadi.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gamwcyaxk.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gzdovhbjf.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gkimreudy.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/grynctqdt.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gmpsmmadu.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gwtttyzjo.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gscaobgbn.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gzntcgfpl.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gwzpiflqe.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/glevipddz.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gpjawnmxn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gmdegluzj.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/geqdytdxe.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gidfieaiu.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gdpeylshi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gqrqklwra.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gemrlcjrv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gkdgoruog.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gvayychpr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gjikixpnh.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gxlqriibb.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gxvfakxng.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gzbwoygqy.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/ghxznzsai.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gbnrrrjvj.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gzvslmajq.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gnaswheho.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gbvdsilbk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gvwvxzvvj.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gadtwlyia.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gafhubhnj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gokqerpnl.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gvyhniamp.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gdjwhflkq.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gahdmcvan.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gxtaydgpc.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/giqhgomai.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gblyyjtkc.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gfqgihxvk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gtsbojqvt.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gtmptsiws.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/ggcbamtmp.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/grctwfjbj.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gwjcngtxg.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gkvcirzkh.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gmazcfkuw.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/genklgfmw.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gpqbkwwwj.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gjgrjguby.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gsmkrrdub.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/ggtadxjxf.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gzxshiscr.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gxjdizwdp.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gkzrchecl.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gdyfieonv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gwnjftdcf.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gjszhojsm.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gktwluymm.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/glkmidmuy.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gidhrnsbs.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gamirxbmy.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gzvylxgnx.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gldxxugkq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gliqwrrfy.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gjuyqpnjd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gapwzzvsq.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gbfwrucos.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gqpqebeth.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gmbzvvtph.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gwcjyxtyb.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gkixytqvh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gyjfgyiro.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/grdaprgwu.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwvzuskfr.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gmkwxbobz.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gqaztqzko.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gayttcppj.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gooeoydou.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gbhuiowsm.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gcafvgmsg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gzmlufjsx.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gmsiaxohh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gvrnpjrwy.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gxzphwyab.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gvdqqfzfg.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gjmwjxewg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gxokhpnww.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gxbpuppyi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/ghaljgsra.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/glnkwcpjd.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/ghajacfzj.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gbazforvi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gipqzrzxs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gybyekajt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gxjqjamlv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtttfqifx.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/glzjwfjzl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gcofiznxx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/grfrofuou.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gcpbotzjh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/giqertnmv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gzlqanneq.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gavdfbsle.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gbonejuqw.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gfxgaadur.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/goxzsxczx.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/grqfzeoyc.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gfaxsklgr.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gdlzrjwwm.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gpfjpllsv.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gdcrzzfog.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gwzudfgoi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gvuxqdgam.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/guykwxhus.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gavsdnppt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gtcbqrivy.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gqyubfxls.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gcosifixv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gqkszbldt.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gfozopiid.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gdvjkozlj.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gwdnmzlxb.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/goimdhisf.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gtfyqfsva.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gifnrpock.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/geewygkbz.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gcmtktadh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gkikfzzmp.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gjdkefwgl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/grahbwtxq.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/ggmkostwo.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gcabzmgve.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/ggtsrdlxw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/glujqhrnj.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/glbiksknl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/ghzzbpjfj.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/goupkuwmy.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gesylegzb.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gnkijdhvp.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gidicoaej.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gvxihaglz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/glryiebkf.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gkihmdxqf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gsusvdwvt.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/geogrfkng.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gsndpacoq.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gwdeqraqc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gphewszge.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gpnxzqbdb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/ghbhblrnu.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/goliuqayt.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gnllbxalh.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gmjhysmky.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/ggufxgchw.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gwfnhlwin.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gmzlfkbaa.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/ggpzqhuke.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gklynkata.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gbpvkavda.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gcddwqkjs.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gogimmfed.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gelhqjnfu.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/glhcrbyow.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gzuibvmka.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gnagojadc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gupvgacnt.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/grdfzjeax.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gaqaufjbw.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gdnjzmmff.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gidglqvao.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gnptctgsy.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gmzyrkwbm.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gahfiksnz.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gxapthkee.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gybrssvnz.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gyrhapkol.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gdbvsfxvu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gsncwggrl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gidnkggyl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gkqmlqzbl.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gvvrjieqd.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/grlwqyszt.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gfkznawwo.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/geexuawnm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gvkzjbrfe.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/giyfnejrv.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gilcwncvo.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gppcwzksk.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gwrnnrjxr.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gdhloiuro.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gmqefyfsb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/glsuiwgyc.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/glxqsmmvl.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/gogmcvtok.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gzlhqhlcn.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gjzyjgegd.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gncbrolwd.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/guofobkqa.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gpwvgwhhk.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gnnphfkqx.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gnbovnxwt.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/givpidiju.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gweufmlsz.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gfzgdpheb.sHtML


<!-- 参考信息 -->