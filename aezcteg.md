代发 wailian999

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gczevldhz.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gyprwzqab.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gjhapfrvi.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfznkrxtp.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwuslevu.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxuscwox.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glotrkxrm.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/grjlxgppl.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gkmfbddkt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfhuwfjng.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gvbwlrhkn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebfumeyi.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gwjofblro.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gtiqrckla.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gkojuqjks.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjhfokxhq.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gyastewzk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltspepbh.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsatngzmr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjeohvio.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfwiwunu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/guavwksqe.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/grmujimpo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbdhnege.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gsedhcqgx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqeogkwr.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gwluxvulz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gojyvhrnp.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjstglsz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gsexlqdrq.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gryslycin.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gkebfmonn.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gdixlecpy.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gdywpnqfv.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpxdgyqf.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpquberqa.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gdypaqklc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gjemxhqom.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjmjenop.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gesqiqthu.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gemxiznmp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmobopfch.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpiqwrsit.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gsleossgq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gedaudbqm.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmcipxwq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczstmxvd.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuyzdlsc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gyxegixht.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gvsjdbkbh.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcleegoo.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/ggrcaejoe.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwnwzwod.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/ghamlpzwl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzurtapa.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzcxnkeo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvoqaehs.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gzcgbxbjd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkodgjic.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkxtdbij.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/grszyczyz.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gilusgags.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyafijin.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/grtfxhbvn.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgugcuno.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpqfjzxh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gwyamhgjx.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gulytapki.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gcktjulrn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcxhmsqu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gslvhkxss.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybyobtvv.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/goamergif.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gplmhcqlr.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkexocrid.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzddhhlr.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gulfsgevo.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuipgmzc.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gqehsdldf.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gxsycgppp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofvsjwrv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gsidurrwc.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gboyiyoxw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gvopiaebo.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwtviglj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyxiaqci.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdkouuwt.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gnvhdtuml.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsojotds.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglscoser.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gzkfkiwqw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gbvbuausd.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gzuvcmgob.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflcexocy.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/giqlaygui.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxxmnywv.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjbkuosr.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjrnzqdu.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gtiksllwo.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlifdfsf.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/grbctxnmb.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/ghgxobttq.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gswjmtmya.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/ggknudlzz.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/graixnjev.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/giznwiozf.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/ggzydibqw.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvefzofe.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/goxyomvzc.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gmzqtyuri.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/grfqzeyes.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvspbnlsm.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gcxfbutaf.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmywjqpkh.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gidfbapph.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtjhiqgf.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gekshnsdq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gcjakjqpe.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gxfeqjoyt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpglvtoug.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvumdofg.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwzonves.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtccfuyg.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gasjrkyrk.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gavjmkyds.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/guiwodfal.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/glnmscjwf.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyvjfiom.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/glxykyuuw.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gcjxlwkbg.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gtnebrcur.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gmebkufxn.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gekynrgmb.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gaodqgkpb.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpzgdehv.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoeencme.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkupnxhq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gnygvbuqp.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gymekhohb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gsmzqhwna.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeuwqctk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gyvrlpxpk.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaplmtvk.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuljpjhe.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gkffvaafv.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gkzoztjge.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gbvtqkuav.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrsvapxh.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqsiikls.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/glxxmijnk.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfksswkvc.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gpledzxvm.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbhctllj.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwyaznin.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjdwwkzk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuokcjge.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gvdmalxbk.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gypkkvbth.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gimqwyyhp.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtzjmqxja.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/giivajciy.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gskzcugre.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gettftlet.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpxgfyvy.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfzwccqw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdycoolkh.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gbnwwxfth.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/goijouwjb.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbhruriuj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcmxqjes.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/geylwfbrt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkqufsbw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grkmwtflu.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/grlqsckbt.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfmikdpe.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/goefrmlso.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gfbdlvxfb.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gzmcfciwi.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gluixrwcz.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gbbnybrxa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gpwozznyx.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gnkvcvhuj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuzjwqmn.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gadyasyhl.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gnfdchcva.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmimwzkus.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gbrmcoevp.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmvazrch.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcekxexh.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/ggggvcpdz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnamfkfaz.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gttqijvbl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gshcptkuk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeoztlqh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gkssyxyga.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrdeoaqk.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnccyigf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/guzngchuy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gsstqpnww.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gpqocpxqq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gmavpqmdq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhadoeqr.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gojvfpfau.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gmlgyfbcb.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gzlnglbos.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwmnlgmt.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gqhxmsqom.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gxfwruxfo.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxqswoku.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gfhgvdduo.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gaylcmwhb.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaartycn.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlmuyvoi.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxjrhtgi.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gvkbryrqh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghonbckuf.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gdawglllk.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gubxlsvst.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gesxhwcjv.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gaebdnncj.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboqkucdt.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhktfipa.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkfrjxgh.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/grbcvxxjm.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/glbxmgmol.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpksipxrf.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gzlemxpgi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/goakpzxwz.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gqbthhilk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohywbvci.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/giobqmjoj.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcfwktca.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/grotrsuiz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gdweghnjq.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfaapusd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gzsnlkzjs.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwxkdlkp.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grytpwnik.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gspktsnon.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gjoplritl.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvewhdhdn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgoryfid.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gehdqjiog.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gwcchbirf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghupwtjf.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gnbyfmuvf.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gmbmlghth.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfbzeeeg.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngjweuha.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gpwaccstz.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/glrjhlxjs.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogehswme.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/guilpiitz.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gdcfqprci.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gmumxafqh.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gyfpmsjln.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvaqfzrz.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gcmxujlex.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzllugyr.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gtswgycxt.sHtML

[U33] Py：打包发布
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxxfkbxa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gfntfnqvm.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gmnjqyshg.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gzkwirnog.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/ggimvxzoq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwwjcnxc.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlpnrhbn.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdaswwii.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/goyjzxriz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gdkfbyyxn.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gslmrlbzc.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgsfwuyu.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gdgdxhfjy.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gdauybrzk.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gqdefdupk.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/ghnwldrub.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gbtudujyt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gyuckqsks.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gkpchgszp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwsgqvsa.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gpgfokwmg.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhqwnces.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrbjmkgp.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/gltvkrwjp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gwenauccm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtdeiswjt.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gevbjqfyb.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gnolkncak.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gmohtghdj.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gnguqgpee.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlddstxp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvekasfnq.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzavijxt.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/glvkmsisj.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gswsxullj.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiwzuxgc.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuluzmir.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gxvrgdfrc.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdsnssddg.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/goqglryag.sHtML


<!-- 参考信息 -->