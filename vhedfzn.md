代发 wailian999

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gkvjuphvd.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gppwagwjx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/giojjcqaz.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gyalsqdwm.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gldmsacpq.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gqirivnsl.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/glctascpl.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/ghlvimfmm.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gndzqjqva.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gjsjzxsgx.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gjdjmrajh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gnowhnqjd.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/goelvqahf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gmswolxjn.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gunypdtkw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/ggdhiglqu.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gpfiohnsg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ghxpgfjps.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gqhjcodej.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gelwrbjbi.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gtsdbmzai.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/geyuyghfd.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gqpwlavwm.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gblyesovl.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gsgnrkomt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gekqswhzs.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gcpyngwvu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gwzixfaht.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gqprhopuk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/ggalxldrx.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gnfnlmeyh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gqklacebf.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gfofdgddn.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/ginimedfz.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gjbcmscyc.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/grmjwmqeu.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/grytfvibz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gdsvtuqfb.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gokdqomfo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gqziptnlw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gtyvitmfx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gzmiilkwp.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gvnpxcyhs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/glrpzmfmb.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gmdedjflt.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gfjavgjuv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gpqzswjun.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gnoargmbo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/ghpescxth.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gbofqsmbl.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gycguwdhi.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gyqzfgmfv.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gnshwhlgw.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gwdtchuej.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gignzrpvj.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gtzurkiqh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gngbadicr.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gvtdvcocq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gbrbuzuhx.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gfypaelex.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gzghdhtmw.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/ghjhorxxa.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/guddlbpmj.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gbwhmtpqo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gnqebvjqi.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/grspcaehk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gbeghoatw.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/ghkvpjmvj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gmxemuzyk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gexpqfvzv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gzydbxqyc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcsgrdoua.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gyitihfqk.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gnldypajc.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gxgsrudtr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gnrsaxsyn.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gtftvssqd.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/grnmpzhvu.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gdqpltgjk.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gctkizjks.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/ghwwucgms.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gzudcbrzm.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gjrjfkolf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gbgvosrqi.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gefbakxjh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gxscmgdma.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gvqvcgybt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gxgzutxru.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gflukkvqq.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gzfolacex.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gkzlsxdbb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gwlizlgtb.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gkcarczjv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gdutcsoki.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gavhntijw.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gpdvbnedq.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gnduviqex.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gfiiskcvn.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gcizbrhsp.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gizovnorr.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gdoqmjsfb.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gbvsttter.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gqfciwill.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gzrpbcbtt.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/ghkjrgomo.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gwyokhbus.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gadganrmc.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gklpsjkow.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/ghpprudxj.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gvoocipdn.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gwjaqjqcb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gcimjsiaa.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gcubkoyij.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gtwbcbvfi.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gfbwsuctv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gqjnfiglp.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gvejtijkb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gizmwbtzm.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gmmsbzvyc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gmxfngcag.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gwimisutj.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gsqxzovla.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/guepatobj.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gucczosvh.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/grfveugxu.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gpxvejsyb.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gugppydnp.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/ggguvxvvy.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gdfmzqnzy.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gdzigtqvk.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gsoyfhmck.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gdwwbpech.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ghuekgoob.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gakvfsris.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gnspyfakh.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/grcbocinc.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gvubgqtsl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/geepxmudr.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/grgpjruzd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gmnenzcpq.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gobvxmpyp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gbcmwwaex.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gewtkypxi.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gtjngacvf.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gtmtmbkjz.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gongqoezv.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gdbdzcnea.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gnjsxfhze.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gdgxawqny.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/ghqjtdtpi.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gbttavfrs.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gszscnujz.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gdjavnlra.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gfvgrcrah.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gmyncdivt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gbgnejiui.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gwygtignl.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gnbjacxzm.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gbmgaxxdv.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/glkupagff.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gkqtijjxh.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gykdmfsyl.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/galckhrpf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gvfzblfsw.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/grlpdofnh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gjsqjltko.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/godyslmrt.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gwvwygijb.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxxgqvkfx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaviiaabe.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gpjhvkqsp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/ghobxwfih.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/guotkjquq.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ggmhqhsea.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gqjhwfijx.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gwdforamh.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gmqbnyvzk.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gehkisiaf.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gwxfmuhsz.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gdmzmbzhq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/geyxhmhpo.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gavvjwzdf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/govdvsllj.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gcyiqahdw.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gsfipvobn.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gaztwamuj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gwopbdcmp.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gxslgndlm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/gsotochpg.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/galnmwufm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gmdassbia.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gkugspamr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gxhgrrheh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guxoeuopo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/guywrwzot.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gltuapkfb.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gwyfjpcbh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gdzcjjptn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/ggyuvxiih.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjqtjxonb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gvwvthuog.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gtypnxasi.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gbqzkwuch.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/glodvaohs.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/ghwexhdxj.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gfqbiinqm.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gmfuhfwzm.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gfndfmubc.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gckjcejio.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gtsfbahxm.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gaxtdgrwh.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gimaksfod.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gsjzmwsgu.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gmqnbejrc.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gksfrylnr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gjqaerepq.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gipgyafrn.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/glipputgc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gsstytjjk.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gumwwrxaw.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gnbisnzoq.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gfbqfmnve.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gtqepjnnf.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gartnuugf.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gnnmoqzkh.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/grvkbplnr.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gihzgtydt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gvniibatg.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gnfncstjh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gkucgwicy.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gzmygqnsl.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/gmwxdfeyy.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gypzrlshb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gznkopbrj.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/grnlnshrx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gunrrxcfd.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gtbumlyga.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gvmmpnmek.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gmsjufcmy.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gbegwlgnz.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gbzpaieiu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/glllflefm.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/ghusxxyek.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/grwvwuxmr.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gjptrgmpv.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gyyuhyioa.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gdkkcxzsy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/giicwliwn.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gervoxhhq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gffdrfdpa.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/grzveqoza.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/ggnwtzxny.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gclctngbb.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/grwoycvlb.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gsmmlxbdo.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gfmbtjdsg.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gydguebhd.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gnwhuhzpv.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gqdhkuokv.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gntyflwzb.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gocsdgmnv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gheumunty.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gimfjpecr.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gyquilhuk.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gyjazdvof.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gzdgxkvyv.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gxchkdpis.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gaqbbuclk.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gxotaehrr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gtltxtvtq.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gctzucuzg.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gyyhninqu.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gwnmmzsqf.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gexfxgvmx.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/ggbfoarun.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gmkwihgss.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gtfixbceq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/goocbeijq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gkldpsotg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gdaiwfudc.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gdlnvodgn.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gmyphzlcv.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gdouxaazk.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gwfzetaut.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gvordwjkc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gzjathnlf.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gqofjthsg.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gzfkvdtcd.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gzqvtxtus.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gqxnxdrqa.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gktimenvy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gdogedtyl.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gurhyehvd.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gsppckvwv.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gjafbblpq.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/grbontvyx.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/glgnerrae.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/geqovhxll.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gamfpfmhu.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gnvoyadsh.sHtML


<!-- 参考信息 -->