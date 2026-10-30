代发 wailian999

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gmqclivpk.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyywwthg.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvwpqcou.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gtgggjttj.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gjijwqcvs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gutsqbhqx.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbtqyhad.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbsrkwtc.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gagvethsx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ghcyhnfbv.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/guskmviwk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzxroahwe.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeoxzgrs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gptqylozo.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/grdkqhpty.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gnvmrbyqz.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givodmcjk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/galcrubag.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gdkxpjvol.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gazfxbqfc.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqhlswvp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyumvlfjm.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gkgchdhdn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gysykvdqv.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxurvlkoq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gsnjrjaua.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcjgorxy.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gdcqenmjd.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsueybyc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwculhhit.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvovaxbx.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghztwugqg.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/ggsrfufkk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwcjttcy.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gkeiovczd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkspztxoj.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/giphsqmrt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcvrvafyh.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsarfiguk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gttytzpsc.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gthmgbfvz.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtukhfucc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gznhlnbvs.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuzcqgoa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gawlpllnk.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzugmrpg.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gmmmqrwea.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/glgxgdpte.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gquixvjhl.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gluxywmit.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/geimwzknn.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gdfnacbbj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbkhnzko.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gobmnmofg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/ggahilmwr.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gzktsexwj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gstbwdrqa.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvivxlqjh.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gpltjnwgj.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgqtszks.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/goywwojzw.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gggaftbxm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gowopxmna.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gepehvtei.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gctltlmmn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaclewmq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gsyzwpkek.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjykudtw.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gzwqcgvzs.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazkebghg.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcriisxcg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyhkwcby.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/ginxynofh.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/germqzivf.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gbhkkajni.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxviqqel.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkrwsyhh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeudgcgl.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytizrtaj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/geghpzatr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gduzphxsc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/giitokcuf.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gypdmmlqx.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/ghqxwjoth.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqwdobok.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwllmtbih.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfejwvld.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gagvhngtf.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmoljubr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqozecelb.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyvmhspb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvwmwjhk.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gavwdsnxu.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcglmzpk.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpgpinrn.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/grwxrngdq.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/glzozispy.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gtyjekium.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gygnbribo.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfnuiwkh.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gazpzxdmz.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gvhvlqlul.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcagwaplm.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyqiusuo.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuprzlyx.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gteivqrgf.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gojzirzmj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/glxgppxvn.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvzvttwv.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gzlpyraxd.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gvargddpn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gdqwpeuia.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwxnskka.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/govqshqqq.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgfzpijf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gckaypunq.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gckzifrbe.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfyklclz.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gxemticoq.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gfsxvbgyp.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gwfopzoxu.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxfyubwu.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gpigfzsig.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/giagpgvsd.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqgsabop.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gdvatwzaw.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyqhdenl.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gewiobvlk.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gfjkqespm.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwhxqgct.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbzpufje.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/govhhdraq.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcsaonip.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gavvtrkym.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfflvtmia.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gshcurxuw.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gzqxknejs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpnoxthx.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvhqeypeq.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gusobblza.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/glodcrjqm.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkgnbdzi.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaapxssv.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/guvbtvxpa.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gyuknjrjl.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gxevlwdgy.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/ghepxvczu.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/giwogvzav.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gvkgdplhl.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gwkxoswpi.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/ggahauvvp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/giboujkqt.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/guqqocvfx.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwimzvfu.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gneaqkecq.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghldnimlb.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfvuvkmp.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grbwujklj.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrihrzdw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbdxxkie.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/glfhfxnmp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqefoyun.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyijvqck.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfzrdlqs.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdtiedmjf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnapjyfku.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcqxpusgv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnqxfmsm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtnqrukjx.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/grbvyywcb.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhlwinld.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtzlxxxcg.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/greycdfeh.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhhxzgvn.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gncxmwyfk.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gszkhmkvb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/grohgbelm.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvllszlsv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqcusoyi.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gpzbfqzfg.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gdimpxfms.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqkvoona.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqlxfcbg.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gnixbyvht.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gjmipaomv.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gsndgeqto.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gduspnrlr.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gkdnomoef.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfvvptyc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaegcpkrz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gfkkemsjp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/goovpqmhj.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gijnkoppn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoshraqs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgbmixeu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsclwjmef.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxmrzwno.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpthjvnd.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gprcgqlgg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gubhxghgh.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gjcuodisr.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruuzkqte.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giammwdaa.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/glqooxyqd.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpjrkurl.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gxrdkrkuq.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgseydvg.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gpaxyctrh.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/glffdjmnw.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyidiqbgv.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/guczsahop.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gellkcptr.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfknmlgl.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gwcalnxry.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gvejmwyjz.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjflfxlzq.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gaesxhgrm.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gruesxdan.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gapnljqgh.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/govkgmcjp.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gfluehjwd.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gwiluvuyx.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqudpcchf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjswmppfw.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/geihulbfs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gshjqjciy.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkmttcbi.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gkdcoblbl.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkvsjfzy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdmdyadr.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/grzmyifaf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxdctqku.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczirwgfn.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gebumvixy.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhfxdtgk.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gqhaadkic.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcaiwslkc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gydrozjlt.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfetnjtz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gnysgirgi.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gfwrkvdku.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjamquart.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gncsakkve.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gzoojvojo.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gzwchnuzy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gusavywnf.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsdirxou.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbvyexwx.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gsfrctgqh.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucftqvni.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsswsuro.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpdiqwkl.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/goadtriox.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrnelhlw.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/goctkgard.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/geprtxwtr.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gzattueea.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gbxwrupfs.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwakxqfjg.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/goegrurqe.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcawqcjlj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gvjyetldo.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/grleuuuqu.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/glyxyrffh.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/galrqazsc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gvhxueppb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrewnwmz.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgxvbhgw.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gldzkocyl.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/glaahjtyk.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/ggxftypyx.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkmarzls.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gptjqvxit.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fanxiaobao.xyz/Article/details/gjcubaitz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gjbzwgndk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniiezevq.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gzeimhmfg.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gejwhkvxs.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gezojjhdc.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gawjiiqgk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphwytlgx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/guqvpzfzy.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gsyimjorn.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitedxzjp.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/grgnlsqiq.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmqligcz.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gjakhrgcx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjsizndhc.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/gnodairpn.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyruyvmdv.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gywffobzb.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gwtwrppfa.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyxkdksu.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzsvzhfh.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gquznufmt.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/grnvggati.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpmvegdw.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrrrmrfb.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goawuwhne.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqzdlptq.sHtML


<!-- 参考信息 -->