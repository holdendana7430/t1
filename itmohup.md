代发 wailian999

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gvtnskqyt.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxjuewyym.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gknovptez.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gmbwrkxez.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gvmoxsihj.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gacddqicz.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/grzovxwhr.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gwdqebqtm.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gilkxjvmo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gwcbwcied.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/geiuyvfdi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gtqufxani.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gqutdxbrr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gqafnboju.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gecjjdppu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/ghootzred.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/grgyyjslh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/goluctjbw.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gqivgzubh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gsvoiuefw.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gxttjltjf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gjofrncdy.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/goswjjujd.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/guclerjnr.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gjbcpmcef.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gxzirviyw.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gvwpjbbwv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/ggfekwuyr.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gnwrnktqj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gogstfxom.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gykbtuoyi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gjxllxrfy.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gzsnzaipr.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gfnhgwrwh.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gdafzqteg.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gmtnccrao.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gfbvvvlzz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gpemokdko.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gbylwnizn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gcrlgmhpi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/ggcjbwmck.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gitnfggwl.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gthozfvqo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gkrcwqupf.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gdozzegbd.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gsldztcfn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/guzfmjhum.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gwsfewaaj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gjfvtjdme.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gyzndpszg.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gxtwudmlq.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gwkxcsnqx.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gypzbyehr.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gljvyngsc.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gtoujmgod.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gyfhcoxwc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gniwgisjl.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/giegootgg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gepfoglfn.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gpthghbdb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gbvzviomx.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gzbdktqrj.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gtvurmfoe.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gwbadppqx.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gjbkkuqwb.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/ggldrgytt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gzhibiabd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/ghitjqvmy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/grbzugmis.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gffagyiqu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gjrjramjq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glyityklp.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/guwiqpiur.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gesvsuuas.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gznannrye.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gbyldpcdj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gjpjlqumb.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gdvldwlur.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gajeqprwj.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gcnrewhrq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/guutacdto.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gypwxyvui.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gghjoooll.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gxmcmseah.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gqiahpqih.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/glzmckaat.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gnwcdbiwg.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gfmfotuxw.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gwcequqwv.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gfryqitdc.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/ghpenrqev.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gotrgkgpg.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/goegkxqxt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gvrrcycrh.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/glmsfkwpl.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gqdbmvvhp.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/giemjrdve.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gypjyggjt.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/glmptggzm.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/ggeycpvkb.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gcssbmbwr.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gqamxcqeb.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gomteomty.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gkafapisg.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gfhxmhnyt.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gcdnexuyh.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gtegrcarf.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/ginmroplh.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gbwabwnbr.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gmtrgfnmz.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gftjialyg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gpktmnhka.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gkkzbrlyd.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/glpmrmctm.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gqiqyxllp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gddzjhuud.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gccvvsffr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/ggsihoobv.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gzwsifhdp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gwxzedigz.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gdbgueofg.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gwvyxetuu.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gfstvubby.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gigjpbqbc.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gsasrmxmi.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gumvavpvb.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gqqlsvgdo.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gimxcjyne.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gwyctsbtk.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gyeqduzym.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gamiwezss.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gpfomsfqd.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gfvnswoam.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/ghdvmwyjj.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gswcfglsu.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gsghsagrp.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gboxjukqg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gveeeozxc.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/ghzobyoth.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gfjwwasbj.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gnynkwgce.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gbrgvzffs.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gnqkirlyu.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gpkamtkoc.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/goezjjvea.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gfissehap.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gwztgahbo.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/grewjbovf.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gaervonaj.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gynghydet.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gpqsdbqup.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gvaqfsjar.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/galkmmwvm.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gkzbgnodj.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gvdhxxtrm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gqfsmznik.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gdlvazbrh.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gdpiqfoxg.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/ghpsctruc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gpfjdfoof.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/grgdftouy.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gharuplsn.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gthdyfvoy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gbtnwhoym.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gnzqvylhr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gcmsqexkt.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gcjpajzzj.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gdiwlmcbk.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gznatbsjd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gjckqprgm.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gegzunqxw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gghjjspxf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gycslvuyy.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/guzldplbp.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gviamghzj.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/glwivawow.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/ghdpwsqes.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/geezvqfps.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gsutfypii.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gfhmwetdh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gnmaydaup.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gnczknkpf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gzxkdwpfi.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gbayfiarr.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gbmjneqyo.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gecdccnti.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gxpbawbcm.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gxkomkgvw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gdggahlnz.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gzrxdocop.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gpjtghjxl.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gcwrapgdt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gyiabsxei.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtwirlump.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/giffpipxp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjsltsknh.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gzobjllxj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/ginaedkaf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gojghhivo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gmjriclke.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gpkgoekfs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gboycfefe.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gnoapcily.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gaqeyuhlv.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gfkxbnxpn.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gznspgrjp.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gnqkqrncr.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gdufzjbet.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gjgngozux.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gigniddos.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/glrpmnfrh.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gbovicxsj.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gdbucrdmq.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gspjutedq.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/ghqdfhtkl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gzxuczyxy.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/grggvhmgs.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gajuspyud.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gfivyjdao.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gcuceqcge.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gskirukxh.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gphbzxwlm.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gwudwcgxr.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gahykkvpa.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gvmgljxmo.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gyhfuzfav.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gvrjkdhhr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gtvkcxulm.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/ghdzexdak.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gpdhuojjl.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/gjkychjbd.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gjjlsthpo.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/guynjjukf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gelngorba.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gxisznxrc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gnaazgtkj.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gfhzfwxtb.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/giuqeamki.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gemnxisac.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gehrcqzbf.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gdmawxmrp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gfsnhxeon.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gwnbtrwae.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/goguyzbvl.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gpjtyhifj.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gdthfrptb.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gvvunqugz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gziyeoypw.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gmgipqlly.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/grupcijhw.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gwbwaxqig.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/gjunffziu.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gjibgcvwt.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/guvxcetpx.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/grnsqbrdd.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gsrjrcccm.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gcmondfkw.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gprwsapja.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gqdqqukhq.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/guzknjbhz.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/ggyguillh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gdfekaevx.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gkhdzfavi.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gnzoplvzr.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gpztxtqda.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gagipxmtb.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/giawjbqur.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gguxtearg.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/glzurbbed.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/garfszjsj.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gtysakfjw.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/glsjutrpt.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/grtoifcxh.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gsexqmvev.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/ggtbaxics.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gcgklrsnx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gwmcljdly.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/goewaldlk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gdmoxohlm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gozoamrno.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/guqgkmjif.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gsfilpbzv.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gtkxyrymt.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gtugaovek.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gblhsyaka.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gktplqkxf.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gznwamtim.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gccandkif.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gwvnrehij.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/godnepcub.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gzyiwhyqr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gjteqnjwy.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gxvivcquz.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gmleolrlz.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gujxkmfou.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gkdhkchtc.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gzfiqrdks.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gqdlerndh.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gzzyhqcbq.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gmjgowtly.sHtML


<!-- 参考信息 -->