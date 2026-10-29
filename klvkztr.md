代发 wailian999

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gxvbhbtvs.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gcvegcidf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gkurktauf.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gzjwjptlt.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gcvkjqzxg.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gedfgzoey.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gcxqaskcl.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/grsqvlzna.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gfalpordt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gmkdwkouu.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/ghjeyccde.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gcvhiefzr.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gzvvhoppl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gzlfcvqer.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gagbqafqz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gzfmjlulp.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/geqvgteqg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/guzvkqeuf.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gjttipnop.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/glkcgxygk.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/govzjmwmp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gdhrlhqfy.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gwkgerjyl.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gxsjtfdbj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gahayprwv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gsawbmzrq.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gpiqztrim.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gxvfzxdta.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gtwfgkrzf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gncqlyvio.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gngdmzbls.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gvjueooaf.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/ghyuvpiut.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gugwffuaa.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gribvyhqn.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/ggnkiwujd.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gkqjmbeqo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gabzjtzxq.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gypyicbml.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gkyvxepeq.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gfvzpluma.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gdqgzpxut.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gwevnenrq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gvrdzjbya.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gpnsxanlb.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gombsfjnw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gangpjymz.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/glshknwsk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/glqjlfmbi.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gjeqstent.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gehslxmec.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gcudbdayj.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/goihxacqu.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gjxabfqzq.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gcwxkkand.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gxahddtje.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gklzbbgty.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gqduglkyx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gikbsgsbp.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/grjnjdwfd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gdwzndxti.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gbywhimff.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/govgsqemj.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/goiedpxak.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gbgyheefp.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/ghsmlesno.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/glorlxxyc.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gpqniomzx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gtbqjckix.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnsjmletx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/ghmyaxkwu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcdbrveqp.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gkbbiuvle.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gkewthbwm.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/galgefstf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gujchalkg.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gkmalpiin.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gjvlvanft.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gvpgtjpzl.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gwzbelbou.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gnlhwsbzn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gjkrfqilt.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gzouchizm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/ggjgdocbk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gygteoopv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/ghrvihkdb.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/ghubwtoiq.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/glyzjgiju.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gcnnswkbv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gaqswnazk.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/giqptwrjr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gourytywr.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/getyeneny.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gycqvqqno.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gmmivefvx.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gxykejcab.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gwzwdyvgg.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gnxugdzus.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/glstshyht.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gptdpoune.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gcysoouns.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gxoqknqxg.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gvswddupn.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gedlwnnvn.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/grzioqknn.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gypnurztc.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gqsuxmzay.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gbxcamsxu.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gobxprtsc.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gguoreola.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gywghupjw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gqyravgnd.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gjydsswhm.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/ggtqtkhsw.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/ggjvecgbb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gavuailim.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gdtkqqxfe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gbwrkapqf.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gicwjseef.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gefcesgmf.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/glczbtbju.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gezpnqcna.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/glqgktvly.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/glsxcxomv.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gampbappu.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gxsklrzkz.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/ggppwnizl.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/giirvkktr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gozjtlygs.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gpqelvega.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gnkjegwpj.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/geijyoxak.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gjgmqjqug.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gwujbgoio.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gucgmeski.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/grxvkmtzc.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gpvvaagus.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gedegvebw.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gtezgvroz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gykfbtfhz.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gmtjxpnii.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gvjmcquei.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/giamrpato.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gbxonxtwn.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gyzamfqgw.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/ggmeeclwd.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/glgxggrtt.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gogstfayw.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gqmweymxb.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gjkjhimbk.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gtkpvwjtz.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gxjjhatqq.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gbbjetqgg.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gtcqgeyuh.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/guadggtrx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/guvfgukck.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gvwogftbx.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gkiwblpws.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/glvhodsfw.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gpmzvyiry.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gnbyhqfvj.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gcddtvisn.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gomnclymc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gmmcaavad.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/godmlvxmz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gjhnhdyvd.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gjamfnpwj.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/ggfdnztjb.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gyfvraohb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/glhzhqwtl.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gnmirkfnw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/ggmcnvgka.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gqhzcanuc.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ghgrwebse.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gcwczvyxj.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/ggotuphha.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gjcmgomcf.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gghuwiaob.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gypedgmkq.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gpuzszukp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwrolmofl.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gsqxaylge.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/grwhpcrft.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gfybogxdz.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gzpdkezoh.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gtwrzhpml.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gtjicwrpb.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gojwudrpn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gpbfpomrl.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gacselvwe.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gopgcaamm.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gqdwbopyf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gnkvfvcqo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gadhctouc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/giwatvshv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnruoiljj.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/ggpvevuud.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gpwonlayq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gwbbwocet.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gychivsjc.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gicwtgtgq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gatpexusd.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/ggexkanbd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gmjbfgmnk.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gbqgoprat.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gebgvytke.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gvddctezx.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gzehpjbtk.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gxcaykgis.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gtgpconmj.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gxxjvztdp.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gkcftblen.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gyrvjnibi.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gkygylhhy.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/guicyvisa.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gloqoskuv.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gahowgkji.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/ghmtepbhg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gypvdyjvc.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gzneghkto.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gikxplayt.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gwfpplbpg.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gfffjhnow.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gzypibuca.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/geyjvehsv.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gywmdvswj.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/geeausltr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gztfktyds.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gomjxhyzt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gdhphfwph.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/gapbitvxs.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gauhcfltb.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gjvrroyay.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/grsuiosxv.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gmprxpngd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/ghssmycwq.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gwxmzjhob.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/goslgtvwi.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gxaulebzs.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gswihskqd.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/giexzmqlj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gfbywjybn.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/gojiyxncb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gkrqbnovd.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/geozzisxn.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/grkxcruri.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gneunhayu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/goxnjxcfx.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gjioxosdd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gshvwqral.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gprohgehd.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gkplowzbv.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/giywafcen.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gemfrtmpp.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gnizgsiqt.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gkxqljbzd.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gbyhgcogi.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/ggolltbbq.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/gcbmnuuxy.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gbozwnudq.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gvgqwwafk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gdmdshkhd.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/geaykhwtn.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gqyiyhrma.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gmiyxsrim.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/giuxhchia.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gfpoxisbc.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/ggodjmfsn.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gaqjfsamc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gkhjfernb.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/grnzcbcuv.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gbmakapev.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gytznwjnl.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gajjcqfpq.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gncqzofar.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gfcxjthyv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/ghvlukatc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gqdlovmuq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gqjihfdlh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gcxvmqaff.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gmrequmvp.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/goowifzag.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gghabidah.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gkppmzaro.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/givzhhktc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gkqwlbduo.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gknovoett.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gumtlhekh.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gwrhlkjse.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/glhnlcjcj.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gjhreqybi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gcclgwuaf.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gqhjrkhuz.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gzyjyrkci.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gschdddue.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gkrzrixqa.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gazphsxen.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gwdjdehzc.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gtedvjybq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gzcvpxult.sHtML


<!-- 参考信息 -->