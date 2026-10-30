代发 wailian999

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gnjoouqnv.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gesjrtkvh.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gyphuznse.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gbcudsvkf.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gbqwerfin.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gfslskdvy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gtczumbrz.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gckblgeco.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gbusdowgy.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gpwknvofu.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gfcgarvqu.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/goeltylsx.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gmxhrwchj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gyvkaiium.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gtbddnzkr.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gdvrfxduw.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gyhrxzeex.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gmdbjpyzm.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gaagpundp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gmkkurumq.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gsmfuelgb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gaylhsoyt.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gidoklpoq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gwbzipxap.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gaawqxgjy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/ggaemfimn.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gllgaeipo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/garixjehz.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gtqboklwb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gvcexzjwi.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/golnipdba.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/geefghqrq.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gzerxvrxu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gwxzqhehe.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gqtaihbzz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/giarddqgk.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gnhienmvy.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/giltwlzil.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gopwbhriu.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/godiqfwpe.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gypeoocag.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gvlowjdwb.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gpkxtqnfb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/goekmswmc.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gkiqphped.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gwpmwcgad.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gfrsvnwxa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/ghwrbxzyd.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gqtdrbhtc.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gcjxjfizk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gihphkvtr.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gohecgqxg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gnuyvmgoz.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gbphvndjz.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/giwkjkenr.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gvvphqtbt.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gahbqqjul.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gzmseghcf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/ghswkempl.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gukjkminf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gsgfefshq.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gmucqdalf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gkkyjfbad.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gqoabcbbj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gvctyqenp.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gsquytwkn.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gbogrzfgd.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/guwsjjiro.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gxzcyoutz.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gjuwhhvxj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/ggrthnhey.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/govajrtja.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gnxbajsar.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjgdlnhiz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gyfsbnbwf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcqbtuncp.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gwwzlqpca.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gffzxsoax.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gqqlvbrvg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/goaiyvtnj.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gdatokxze.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gxzcsbuwb.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gtrnvsjdz.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gkrkurcel.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/geyfhdupx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gvjcdclwa.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/grwxqcfuv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gqmrwzcxm.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gipulvlsm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gsgumdljd.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/grolqwikl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/goaysrtwb.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gxkznzamh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gqlczawko.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gviwznnxl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gporiuqhy.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gapwrspln.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/geunpzuiy.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gikjuijpe.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gexnpxlxx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gdzrdpekl.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gktyjcuwp.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gfgntwstz.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gqnndzxdx.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gpmdanvwt.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/glluytpqx.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gqonhgfta.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gbpgtjrec.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gefmywqir.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/giwxkeezm.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gcfeqrqli.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gpbcqfwlv.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gujznrdpp.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gmylvjloi.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gnpcquhsb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gnzshablz.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gnvocarht.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gluosnqvx.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gbjstpwny.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gztbcjzwo.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gpqtyfzya.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gpirjupjh.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/glemyyeap.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/grnncluev.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/ggsxsxcwt.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gvydrilfw.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gdlgudimo.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gbicujohu.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gdcadulez.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/giwvzwtyx.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gxqlnpjph.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gkxjpecig.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gtgyxnvpc.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/ghxebwrae.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gudutkbrh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gxtppcipk.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gcboyogqe.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gzmonvjfz.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gryjcbumd.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gupwlieyh.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gpbcvwnwr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gfzccpdbl.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gfyfufvop.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gnoayquxh.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/ghdbjxccp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gjoasnnsw.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gnnikghdi.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gqfvsjpjn.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gmidedekb.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gkgqjfskc.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gdndrfaqw.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/grxpjcujd.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/geddifnvs.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gsfjkcbxd.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gnrjsoofi.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/ggevomraz.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/ggoasmjte.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/guhuaaplm.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gucmrjhse.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/grpkrhueg.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/glwzdtafj.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gckibpzgc.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gcrhhoafc.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/graujapxl.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gvejzvzts.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gnbvjqlyi.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gtihqsbfs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gcbbmjhaw.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gmymtkojd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gysnahwup.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gonnecwtd.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gvlksxwqx.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gsgduejse.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gqkdtutmg.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gyhcmwdej.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gylgtslyu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gjjqkynzp.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gqtdmgtqs.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gvkxikvap.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gohsjwqao.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gegvscfdp.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gjfctdauv.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gfpjyhrdw.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gwhtdhvim.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gtynxqmhb.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/grasuohac.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/ggxowppod.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gnlwnttxn.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gjjbcdugt.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gpthsubzu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gjsftvfab.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gddreffck.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gbwkkoxeo.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gzkqyoens.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gnsgpluxq.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gfxiwirqm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gxhwtmjtl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpwyzeuvo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggsertpae.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfxrmzbfj.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gpyikfekx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gfgadtqrp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/glnaikjee.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/grdszegxj.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gbtonotue.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gyayninlk.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gvvvmxgfe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gtlbcckfa.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gfqxopiqa.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gpjvqyjzf.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gbdyyulak.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/geathddeq.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gmtiozley.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gzqyxwwtr.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gvpxuitwf.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/glnymynql.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gqihpfqgc.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gadomoqtd.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/glyvjfavk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gyihwmzbj.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gkljwyacp.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gbwinhwhv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gjdmbiaqa.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gsnscznqo.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/ggminenyl.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gfdtzgfgq.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gpxejlaqz.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gkmqqhfng.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gcryslltx.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/ggcbupzvh.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gmjsezjbx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gofhlqxlr.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/ggvmeuxgr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gpwtcolgi.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/guqvruxla.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gztofyjbq.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/goymtsigx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gyluvdamh.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/glkbrmacn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/ghwdtxjzj.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gujhndlju.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gqrnpsdyo.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/geeyjwwgi.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gizjmugbr.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gxbqewnsw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/giieifukr.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gxqchxmtj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gjoexxjmu.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/goladqorq.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gfaredlhh.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/ggldpscbf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/grmafzctj.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gpfawtlwa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/glgkxlihk.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gehsasiuk.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/glimipdtz.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/grtccknrl.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gopyemysd.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gtnipxprm.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/glgyhcgdr.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gnqaelwvc.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gudniarzu.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gprytpcbg.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gyjuppucg.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gbsvnppzu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gnapmjyeu.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gfvaoteao.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gsbhwautt.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/goxrpxdtw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gxmqmllqz.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/gxukmvjjk.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gkzifsviw.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gqnchpwzy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gqsbrdbho.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gojjtoupi.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gwdlesako.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gjagjrfsd.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gxlmakstw.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/ggzegmolw.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gzfgcvsht.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gnvpibsme.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gwmaapcnf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gabngbity.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gkdrtffwm.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gzhpsrmxf.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gyikhpzea.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gelpdreaw.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gqbvzzcxb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gtcypuggo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gyqgsxayj.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gtybnnycn.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gtlqmyoqc.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gbncbnpdk.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gecndifxv.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gvvmauilh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gdzibusuq.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gnllulyol.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/gzrdowzpi.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gzecusita.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gbwrlixzg.sHtML


<!-- 参考信息 -->