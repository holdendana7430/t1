代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidjbglem.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyewhtixs.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiowwefw.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gewxsgjiv.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsxnslne.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgkjmgcy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/glhuwijvq.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gqputffhd.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gsaazyruz.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmngaemem.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrecwztr.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwyqdbho.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfjtjjhu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaghfdfgo.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gcinowpeq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrzyrwhr.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gavdjbbej.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gtijthvcp.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gcusqpnqm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvqwninlv.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryzdvbon.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjomtrdv.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslisdzgb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnptrnspz.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdohgpdub.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gabmuzfxt.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gjkvdounh.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gaesusplw.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/grhfucwmd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/ghztocjed.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gaoeiydmg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/glnlbvbdw.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtjhphzwt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gngfrugxk.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/ggghbrdol.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gkgnowrsu.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzutatom.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmfryhow.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/ggreayhlp.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxzgshzee.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoferknv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gjhhgmbzu.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmyaoyaa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqefogzhd.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gvgxloqhk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gomgiugyy.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxpvianc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjvzcpsn.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gtjkivhqt.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjtlorzt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gyqbaamzi.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahbiusky.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceonnigz.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvwzpjvc.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpckbolo.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gjqitakah.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfnqkxoh.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gmnmvzzms.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/galwsufae.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gjpbjczmn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsvqutqf.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuhvlpdr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnsgftdw.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeihlwqn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvzrybhjw.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gvokantbu.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdolmyigt.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gdqoawzdo.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gotlzgyrb.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjbtwjjv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcdsloqu.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrdsffhj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahuukajv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoivgucn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/ggyewzhha.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzkjlmxk.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ghhclzops.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhjojvyt.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxjskeclf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/ghmrqyllp.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gsafmsylw.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/glrqgpswz.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnqxwxqo.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkmvfxve.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gqxwaoimv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/ghercrmmt.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadnsbube.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gxibctnzi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgfymhzk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnxkhekf.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gkzlkewql.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gcklgckzi.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbjxddlhg.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsgtumhe.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhafakon.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofscpmwx.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gneolodyh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyxdnkxe.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gwdnnimni.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlnwdgyf.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gtetygdhi.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqijrvsw.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gfwasanrr.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gudyfxsoz.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gopvtvben.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpqggjrr.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwaguzhj.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfimontt.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gladqucdh.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmowuoop.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gykiilyfq.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaixuenb.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmlbjdti.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gqvzkouga.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gqffebztx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlbtuqoc.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gnlefjjop.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnocdzvpj.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgneaaok.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgfzzzkt.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvxbpado.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyftpvsjk.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzojhlej.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcrrkdgp.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gguwjzxjn.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gentsdmpf.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtfkpaxu.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswswpzpn.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeklqrij.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gygwjiyhd.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/glezqytue.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/grkbyyudk.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gdfplcbbt.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gpbaiuguv.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylwpugjd.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/geqllkhtu.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gababarrh.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gshmqitti.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdbtunawz.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gtikfvneu.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvknyumkb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gxahwnjay.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gzznuprhn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gireriyjv.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdbymddn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/guqwyekmp.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzclipozh.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gufvtukkr.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzfbxwnh.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvwseszx.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/grnqihuyq.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcjewnva.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjfarbyu.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gndtpuigu.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gpylzupir.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gajdvmbhw.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gjmwsccfe.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvfpuryc.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gbsiywaec.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gzfalqxqj.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gsocuihiw.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/grwfhscrn.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhyueoja.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfevzffs.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gnulbcjcf.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsojmmwwo.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gphjmtveo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiwciccg.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gmabglhpw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjibcxvyb.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gncjffqdv.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gtkfbnxss.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdeyqurds.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxokxcvut.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpdlnbpvi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnadafvft.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/glpaybxvy.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gpmtgagnm.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/ggjaatkod.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcyzuatqv.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytamanqb.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gnguhjxzb.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqkyjfqz.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozltlnkj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gewzaocuy.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrgcnzvo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gwkolhizi.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gltkirxcf.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgqxblig.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gesbiobte.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfngmflxj.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnfrtcmw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlsxhxvj.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/granmsndx.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsldpnmnf.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/glucshkws.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdanmtqb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gohfhdybw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqkxebok.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggypzllud.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrksumfq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/ggdivuxtq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gudtnatzn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnixnkxir.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzeozvxu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gayterjbh.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gedobzqgg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gojemgzxp.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gexcweret.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/guyzwsfjm.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gjbtcbnqa.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gemynwmvm.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyicyesnx.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzarbzdz.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gvcwhttfk.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcgljnru.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gbahcjoai.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyylhqzq.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqoblwsx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqllljuz.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/ghilosmav.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkyftzzl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelzhwhcg.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvdkcgyj.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/guqczufrm.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gspgjarlq.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrqlepsa.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwznshxg.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gikukcdnc.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkiqrezu.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmepllpmw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxipugmn.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonupacqr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/glrwabppt.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gcrevznxh.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/garilwnjz.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvbkpcbv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/glkkidadt.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngjceffi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/goxnduoqc.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/ggtbrytpm.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimwymxre.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/glbbsoars.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjgirdvj.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcudkynts.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gkvhyhyun.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/guedhjdrk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnauuraxn.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gufizkctw.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gglbsjcwf.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunvklbnr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gihdtadoi.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gbznwszxj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gqnvgqhlh.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhlogmdt.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkmtdysw.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjusgmsb.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gzoyewmfb.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gbliwnjsr.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxuupqbw.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gucgcfrbq.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gwbjjrckw.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqlruxrm.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueqrklic.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoyjrozi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/grtxioeuj.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsywdaih.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gvkyebpxe.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzftcppj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyrvdlku.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocwesgjc.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxiahtlw.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxlzjkfk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gocnkqsgz.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrcaimgl.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gfihuutig.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/guhvgfzol.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/ggysdvknt.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwajaqxl.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflsvzkzv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gnqudldpq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjzpztod.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/giipnxhau.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggulvdpdh.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdsctovz.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyemhsij.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gfhpsaqir.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gjaurvtux.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifnroobt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuhcfkll.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqjsenks.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gvldzgjlb.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gipyqyqdp.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gnbzcffjk.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gmvxdkzje.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gosaoldcx.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtymeezq.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpknygga.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/gykoozxjf.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gsggedalp.sHtML


<!-- 参考信息 -->