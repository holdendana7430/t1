代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3lvulnbax.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3grdvjoje.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3bfnwkpfu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3mopjadmw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3iqhakork.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3hxdzbjkx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xatjtqqy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3skwmugep.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mpljjrnw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3fplvbrdf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3phpjcbsl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3plpcxjyz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dexnihqx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jdzebctq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3vzdbwajq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jwsnptbr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3onximnjn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3vmkasbxh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kxzfuzcu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3gpwldigm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3jrzzqbvn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ezvlzcln.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3mehsqmjz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdixvirh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3tvbdjjrz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sejdumjm.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3yraozuia.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wefigtha.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3tawfzbki.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3dymrgnkh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3coxuffsd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3egtnqnso.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ohkmmelo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qzabwskc.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3rgfihhrv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kewudivv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nrljsqtt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3mdlxdudo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3zykjruib.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3cxxxdyrt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ilfowkdp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3tjyfspdi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3cshlbsbh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3crduixbl.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3tkcyyxba.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3efrcnlwh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3wfstxqhs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgqnlkdx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yhfoegav.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwkjyqot.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uqtdzjkk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3lawynhdd.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uhkuyrwc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ofhoexkd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3nklwohvu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3jfzzalvg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wbzgkauy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gwwasqvd.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3occxcwzt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ayhwforq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3khmbkdjw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3fswvxupa.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cyygtftg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ivgojgyc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3zqbnbcil.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rqfsvcpy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ipslnbsh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3bgdsxjjj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3gurhomep.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3bcrylumv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ugqizylz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ixffdnrm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eskfzyzg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3hjohzymd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3onqjlfuh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cryukrno.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bxeuwpdb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wolgwyfe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3oaigjtuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhdohpxn.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lrvljnhi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gcvntahe.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ombuyfpl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3njcbrkce.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3dosridlg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wtirjgkn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3aiynnwjc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3luhddloy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jmafmmrg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3yzasnwoc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fkbhzdxl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3msrewxlt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mageuqub.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zesgftwe.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hsvxyxku.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rigmvuoa.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3bdsukzwr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3wjrfddua.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3lctjzxmg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qvlrflvw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3kvdpgvuf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3immlmkdh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3lseggvyw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3slzyuvbk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ujukmgep.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3kdajodhh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3qsnlajsn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xisqlspg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3tlbtqawc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3okzlzvxj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lietalmx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mtncevss.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3tlwqcdkj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3fmgncavd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ynmsyyja.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3swgkbafl.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3cebqfatu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3qeumlxva.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3xqmuvfuz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ynckgcfw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ycqljzmi.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3cnvqlccx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3rxrqfekz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dkuyitfs.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3majmmele.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kcxfmfsz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3iowkzywj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zkjreohs.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3csokvjvc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3aeqqfywt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3mcdowcui.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jfkykafq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3cypyixcc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ruzbhhxc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mbflhanx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3vrepnjcx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3aoltqgdc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3dcsmwbjy.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3lpgpgxxn.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ixnnhekr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fqrzynlk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3iivslvof.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3smptyxoq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ijvispjt.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3avnhkstq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ptwymlrq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3lfcifhzc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3mbisaera.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3iikvhbvl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hatlmvmw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3wwaytzqm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3qzimopyk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3esurpynf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3whyedhmp.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3exxaiscg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3lczwmube.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bsroyarp.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3gpkfonoz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3cabdjlwc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3iumpmtxu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3talhnxeb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3drqljxqy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3coefrlzy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3krqjtqoh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hlzdascm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3iblbzruc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3musmqped.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3otzdxfyg.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gbuzoqcr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvwhqvhb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3rdcfigks.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdlufnoq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3qjwffxuy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3zcvnjznp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zrxbymja.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3joliyyze.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3eijzcxhh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xqxzuzas.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mjeicagr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3yinrdkrf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwmrrjgp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gwqhlvfa.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fxglwmuh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3fhvjflwr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ldewslxb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pjidgryh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jteqjyge.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fuvyruoj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ctaykbnl.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lsclqkxj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ulfogmxp.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3tfcuovqa.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vwyfaeaz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ubwrdpji.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3udedjfhl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ecgozxea.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3aiolvxpu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3rfsstfqq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ecmdfmhm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3uswprphk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3aohuvwvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfpmarur.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pppctlzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvhzgblr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3zuhmendo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3zuswxpqy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3gngdvmdc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3dyvimflv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3gkzhxgjb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3lnwcpcwg.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3sdxpopin.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3tynvhfrq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3kxtmdtif.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xycmwihq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3pxzvlbwn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3udlxugbj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3iswdfavf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3zsprzjzy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3cpgofoyo.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ktudxyvz.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jbywvjft.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3lowlyddw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3yenbjpkc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ooplaxcs.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3arvghprb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3blvmvmmx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3hrmxuphr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qycvtemx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3gevaifoq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3scdzfeeg.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ayxexbds.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3fcbbjhrm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3hipyeikw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3rpfljfzd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3upwneggy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3sdsybfjv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3rekcdgwg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3kijijsop.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3aghlafzi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hlwroemf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3sjioduwo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3tnkgjbod.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3sudrfavf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3aeaxdnrd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3lnhlygll.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3sfkdzxuz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3qmoimztf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3lmmwjipo.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3spxuynhs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3hfdabwds.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3urjymtvy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bgitunrp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ontbpxdl.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3zzvacmqp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3yftdyqcs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3hmipsocu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3zfsvwlea.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3acqcmcqf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3qekryiba.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3uwwdvdcn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3lchqpjvg.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3oqbfelwz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3qvrmayld.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qdaytdrq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3oekillyx.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3rsijuktf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3qrnsbtfm.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3jivqxkkd.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3slxfdvux.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3hegbjbwq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3lvszvhyt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3zslrfsxc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3wietroyh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3mjqmfhhd.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3eaiptanl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3mwvfvtic.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3kkluxqgk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3tugeaadu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3auyanxga.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3rbgucszh.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3zshjjkot.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3iexfhgvt.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3juwcdjpa.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jnppulow.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3kxqifdhw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3sncthuwy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3rwcyemng.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3livhbgwr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ggwxfsqn.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3egiqlgrq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3kipichzi.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3fceptsmr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ojciigun.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ocljipwh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3tlkxsfha.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3mfonaund.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3taosqgsh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ksqesott.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3zqdivshu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmyfooiz.html


<!-- 参考信息 -->