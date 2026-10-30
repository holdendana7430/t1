代发 wailian999

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gnxpckrel.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gegrlcxyl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnejlklof.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gmhlqosqt.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gmttjgsfi.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gjsogglyq.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuyofxfo.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkqzvouq.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gxsxpanqk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfhhdmxu.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gpdqewwyf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjdfgodo.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuzenxnh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/grlxtartu.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gpelmxnjh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxzinoznj.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzdhfflj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvzocabb.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gsogeuitg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhqoszge.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnqngmrn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gngqdotxv.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gtstyrzys.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gcdshpork.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/ggnkzgecs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gxxndczbl.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gkduvixlq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gbupzdhxx.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoneehzd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gkwyaqgsf.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkzebhhk.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gogmxjqnv.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpeuxqhp.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjerupdwo.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzewuauy.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcenhguf.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gxlnjgiyc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/guupitumj.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahgxxllv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwcfddvu.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/guzkedhfb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gikkfkxox.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlebhlaj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gnaidgjau.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggujtyqjn.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbszzqac.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/ggxrcwqxs.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gfskbuoxz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/glkvplcxt.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/genwklwfc.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomnrzltw.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/ghmkwcipu.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gidbcovut.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcanmmyi.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/glmmjgwsb.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gqihwqswz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/glcanvixp.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gfogsyyws.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/goochnmjy.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmfvdinj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtghrwhmd.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gbcoygwdr.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gswahgfyw.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuahvcfb.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gtlftlbef.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjgtwdym.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gquebphrd.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqzbzxzj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloadoseh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgyfujeu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grloefpte.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbnbuwzp.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ghumtdnby.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gxskpkeoh.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gfjyndzhn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gkjnvznni.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gadydwfnb.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwfhqlsv.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgkyxdvg.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gzrevbsui.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gnbfdiado.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmcynvrz.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/grkccqelc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/geybhlhjg.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gybbbqhss.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gpkpboaky.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnhfdttg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexitwyuo.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyvmekvc.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gitsrhfsb.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gowkcagmr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gscuiohcd.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/goctdnkmm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gxxnspkgp.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gzfcwkpag.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gobswwrzy.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gttktseat.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/ghpcqzvpp.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gbnoemhat.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gbtzzqdsg.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmlofvpx.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gsfzxrire.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gceityvul.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gflgkjsxu.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gzkehmquz.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gbhvkzvmt.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gaozvprxj.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gduqmxsvv.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwtojohz.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidqrziid.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gbocybxlu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gzumfcdbg.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqctgvdoo.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gehiqdhsn.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gcyraxqiz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpwcrbly.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxjzoznn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxuocmws.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/guxpezguj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gosmewjap.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxgvneqt.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/giwpthgzy.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiaatbps.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbnvgpkk.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gcehpiqhw.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gilhtrgtk.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzskjyrx.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcvsikuo.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gmboetxdc.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/ghvyosvwe.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/guiuowgjr.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzxtikji.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gmgafelkq.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/grboexzft.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garjmcnvy.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqbhkncy.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/ghidwshan.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvrjkxsq.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjnnunnx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrzwrmeb.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/glmopqtdl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcsdgoge.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gygrnuvtt.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glztjbhhf.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gpstqtqaa.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuxxoubg.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gesgolbwf.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/grczcpfvn.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgdufafw.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmucehccs.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhsucahk.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gecghazpg.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gwamrcdtf.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gouxyptdp.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gddruiggh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gkbiwvqyx.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzepwxqd.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkocscjqs.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gctooglzb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybahwzwx.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaegtiyyt.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnltaudfg.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gmsrmunlv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkigahet.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gcnhiipby.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnblkfics.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gdcwbblby.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrsiupjq.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdomltduw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gatrigxxw.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepdmtysh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gzgkyejpk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvedrhpro.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gudfarbcj.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gztothniv.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqhgwmhfw.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gibnkkebm.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiqemedl.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmggvrerz.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlxclkco.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/ghstmhwjy.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkgvghsv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyzfhnrj.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geszrpjul.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/girbihlsm.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gxryadpup.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gpahlgvfv.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjnoinym.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrbtccav.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/glzyzqjph.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/grysxpymq.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlqknjqa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/girkczlnx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gspddzhza.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gawrqcrju.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyahsarn.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeenyxal.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/goqtxbkej.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkqxfmjz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gevjxvkxs.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geixtbeap.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/getzerchq.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gucatitju.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gdhexcbko.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/glnbsjmut.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeulgado.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/ggulioxeh.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gitttlqkw.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grutgbvnf.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gudtyjlpy.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/ghstpoydv.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlqotyrp.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gcotyaaja.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkjhzfpv.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gvbwxhapv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkrkfvbo.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkqzulji.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gmzjwhwtj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gmajrdjbk.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeukpzer.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gszxjlmkh.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gyvekovyq.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/ginrjnkdp.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gqezfxwfl.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giikypeix.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwivztzy.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/giyhpnoll.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/guoxrrejb.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gioqqzxnw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkifqtnzg.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gzwkzhlrb.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gcblfgpbd.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gywfpbghc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gpsjkztbo.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkacvlgrk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzurrohxv.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gugkupepu.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/guoqcwzlh.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/grquohzsp.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbrngmml.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gezrzoxrw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gcvmboovx.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlmhlxmg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfaabngz.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gdgudsyip.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gawltydem.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gixmqyjky.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyffgknj.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmplqdlbb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrgzcbdy.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gabhzhddp.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gneoqhiyr.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gwxnyuhqv.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwevrhls.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gibgkwcmx.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gfbbohxef.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiktwcck.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/giccujylu.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gbzutppjw.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiqjxwjw.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gpwtrdghu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjybpxyck.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gkttifiur.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/grvrrvtoo.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/ghmfpphcb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkwbbxzj.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/giajkrehi.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/goafvxprw.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gfzumgllc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfnimhqc.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfyhxzff.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gedmargdc.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfmwnmcx.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvsczgkv.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijeumscz.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnetjszc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtzojyjt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gyetdvacc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/ghygnxshh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gvgpufpwp.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlpzmdtv.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gyxwkiddj.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlugnjpl.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqesprmx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gfmvsjyvy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeqecwez.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsownqzf.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrxgdyet.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gqdoupxmw.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezdlpore.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsdmwzpm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfosgybia.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gwejuhemk.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpykuqsi.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gnbgkfhnw.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gfllusedb.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhlzvyxw.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gxyqydrke.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvseybcde.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/geqrzccnt.sHtML


<!-- 参考信息 -->