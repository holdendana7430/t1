代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcpehulm.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/ggpyqmwgh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gxarxtvge.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhgyogre.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtneilhza.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydsjftdp.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gollrtqzs.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gungfwhro.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gmtyxenok.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdfodgvz.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyloihaa.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxrsbdln.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gctnftehx.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfmbhqxbq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gyjcdphyt.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqdraaaa.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjwguqrc.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gujpbzbqr.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gxryupdyg.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnwbpopg.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/ggdqguftf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/glpoxnudc.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gttvipyln.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerzyxwhq.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gyjidpukk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtovlkvyk.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gbxgtcjcr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsehatuzd.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gharapgpq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdgfanvu.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/govlciulo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gblwvuyry.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gdndfpbww.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxxroatd.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpuzvgaz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/glohfckxr.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/grpgwtxtc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gqedisnqh.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbltpcphl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gqymoshfz.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxamtkusv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvhqupic.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxszfvaf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuywrlyc.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqkaenwd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqvjubyo.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaunccoer.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhtgiudx.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gtceqoprx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/geqstohoc.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqubhjat.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gohnbfncd.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/guqxynufh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtrkeiar.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gedewytnm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gykvwazea.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gceekztzq.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsqxkxtbs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gwvzhtury.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlwjwmzg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ghgwivvad.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/galfhixdw.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnluvahgi.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiihlyra.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/geozfpfjr.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjnzdwrc.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/geyzkzzmf.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttupnily.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznhujdyc.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbevykuo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyygcsgji.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnylawcn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gildrowaa.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gbvcczgnv.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gowjtduaw.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gnwcvnjiy.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gslcarrij.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlkletyi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gxrqubtns.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gejdhtzbd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gljttqcen.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekiopcsx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzporzhmi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxwvqhfkn.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gatdybuck.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpmuoeej.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcbjnityr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gbhaxlbdf.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/glasfkoqm.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdrwcryn.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqfkpwnb.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gsaxberxs.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gmsihesje.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmluxcpn.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/guvfyvdmh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtwdotcy.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gvzuqznun.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gqfdpuvzj.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gdujqhnbh.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeidpeea.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzmvratep.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/glbpsprwx.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gyzhrrnwf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjynrdwac.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gvmwafcmf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtomzhylr.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpgyqwdp.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/glvkgclkj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgrztkum.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmsdplcc.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gltbccwpa.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gifzitqic.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gcbzwhhax.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxktvaaf.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ghplupjve.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbslqvmb.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqcptbhl.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdogsklz.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzyzezoy.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzovvicy.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmemxknsk.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gakyuwcur.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdrfkocy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoglhlls.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjjixwlz.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gfpqrferv.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gvjmhxdfy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gjdipkiwp.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gapcokgmx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gpcfrheap.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gtatqfnwr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqymsnngu.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/ggywgolpl.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/grbezuelz.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gziibkwzv.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawtwakch.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gczjbozqy.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbrvlxnj.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlvueoes.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnccelbpn.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gxpjbmxoi.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gidmpmydq.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjnobcnm.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gavswbelp.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnwwwnow.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcealdmig.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsautqok.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/guhjltrlh.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/grghirylc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gqpqqfmml.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/guqamymen.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gbtntkacb.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxybbezkl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gugveuuzt.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqbquajs.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gnucubwir.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuhdxohi.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcrptykn.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtstzruk.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gbbbsosyl.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gyposrtzf.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gusowmhbk.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gnonsahep.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gmfdfjetu.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcsskmmw.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfgpjgyc.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gycmymtmd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gmsviyzgy.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmjpnora.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfvmhaul.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gdhbawfpa.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/geitvupep.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzyagdbe.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpaxyeeq.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxjnhxvw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcvbbqsfx.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/grsyqjzea.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/givljfvsf.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkohpewpb.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/glnanowlk.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/giqeypxkj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnavqlsqx.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwakyregp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gfpkqwplu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyudcmyep.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/guooykziw.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gglghaftn.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgusibzo.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/ghhjyvrav.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkxmgqpu.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gatzthvqm.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gbaqcwfrd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/ggtpkjyzi.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gashbyfxc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/grjvydloh.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gpruccylb.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gefworkuf.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gdkxaireh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqjtcbco.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnrdfbcf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gueykxdqz.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gywngkxcm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeklenpy.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqueipgm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/giocogsuo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/guexykgnf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gmgojqsza.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjktbdyh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcolxsouh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/guelvxgpd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gengcjtfp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtqwzyhm.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gbpobtnus.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcnzzwzj.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqmhjkpc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrbgxnjv.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gtzbuohjx.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/ggsokimcu.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxebfbwja.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlcepugs.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkobifogg.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gajoasonh.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/glkitgdij.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/gucmpyjeu.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gaebaskrz.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gqlolkysk.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyyjzclw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gqisfqnsp.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gsclclvvq.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/guefwezlb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gfrjnljhw.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihaswava.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/giaiwwrgk.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggacnkkmw.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/guelodwjx.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyniiyyky.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gtytxyvah.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/ghweehazu.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gmecouoeo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gxuwdsdbp.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmqrxewx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/ghqsiuyty.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoicvzkn.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvuxahug.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gdotiphvq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/ghmnsaxvw.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gcfzsuygm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwhohpxs.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedxypsnh.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gvdlwmcph.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gkqsbrsvw.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrgxwtvm.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvnugkuk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqfjbmjk.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gliivjsxt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gtlirmlib.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnmqedka.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/ginetvyxb.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/gxknpkiif.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gagshmecj.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmeaiurm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gzftajmxr.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gzldhllib.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gittkkkpu.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzrcrcvd.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmuragql.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoksdbgj.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gfjpmgcim.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcshligf.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdvbtptu.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gqzjffurb.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gziyyhxjy.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gilslltwa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtgzqlno.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/goaivmxbs.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstpucgri.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gkxczvwna.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/gekbsvkpi.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gqyigfklf.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/guosbcooj.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqxhbsdh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gczycdzbi.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gfujaekam.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gulzxdpeq.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgyouebt.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxokfmhqj.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gktabthjf.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/grhpxtviv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/giilxabyw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fanxiaobao.xyz/Article/details/giyrootzg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwwgvzhn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgfcbkvn.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gehcjciyb.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtszknxly.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaujykwt.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giywhpomg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gznrhqepl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/glbzzoabm.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwgjyqfd.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gfierfowd.sHtML


<!-- 参考信息 -->