代发 wailian999

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gkjntkodb.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gvvefqvjh.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gowcwrhgn.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gmxdlchbh.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gfkvprdwt.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gpzwtqajr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gzcaxquba.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gnodtwgeq.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gkwragzlf.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/giexighpk.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gdmbaxdtw.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gyidlzort.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gpfsgirfd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gskyfclua.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gevkxpnfi.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/grnmibpyz.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gktmrdayc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gqkbblrdt.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gchsuenta.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gcvedsfkf.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gtwdfhfue.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/geyazqvxq.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gyvfcvpfh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gtooxcfkt.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gmdeihzpn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gtxgajlgc.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gabcifmjj.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/ggydrxlei.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gaskmdhbl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gtcoumqkv.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gmulokohw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gcajogxyx.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/guwibhoza.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/ghbjitwem.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gmjptsejj.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/ggrfzbqwt.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/ghbfhujvq.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/glfhwalev.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gzepokkkw.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gzjmyecsi.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gezggyzyt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gnguvimhq.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gmgrcikbw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gcjhkakpb.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gnmqhgmbz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/guiyzrilb.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gwiltuklh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gsmajskqv.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gmirwwwiy.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gwxnhxksb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gtizfyxyr.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gpostxsiy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gjbvtcaiz.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gvnugkgfi.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gqhnnycom.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gwwsqhefm.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gsvhtcicz.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/ginojiykz.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gkaxzgytz.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gpanjnvlw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/ggcextdhz.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gebiayjez.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gkwjvtnnl.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/goeelabub.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gawuusmmh.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gmztevyvu.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gxubiovob.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gxevnmleg.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gwadcnjea.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gwfuuctdr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gkumlnswq.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gsllsdmkw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gagowuyvu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnyxjwjwe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gjbaywexw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grudijxii.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gmhnduisu.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gwvocpkxo.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/grvchtpla.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gmakljlgo.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gnmtfhrmt.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gewpdbkdz.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gzrxekpzk.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gpefajvqb.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gnogrtgmd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gkavolzom.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gxwomtfss.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/glvgnigvv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/guvqqhfxe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gwtlaswrg.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gskneisic.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gfijhbtlj.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gthqovoud.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gqfwchkjg.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gstvxkkse.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gjlqehjre.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gedaxutcm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gcdtzyxeo.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gljaotsvv.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gwmcobzzz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gpithwtlz.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gthmysbpm.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gtrautgii.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gnfvrvnsf.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gnnucbafb.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gqtwxxwgj.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gjjeqpfbn.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gumthfnam.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gtlrbennc.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gbirqnrhq.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/geubuqfxc.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gsbqtjswn.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gpyemjryx.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gpzloaetl.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gqbejbdwc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gfyetjovz.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gmbxkgxly.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gvmodxqzi.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gbakkyqqw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gyhighqzu.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gpprlnhyk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/gctmgbwox.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gfaeewyuc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/ghcoafmbt.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gbvofzfdc.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gpcnixwnf.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gcfwinycy.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gmreglluy.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gqjghbimy.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gzevcyhtf.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gbnopzgvf.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gygwuaxfh.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gwbzjksdr.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gztwwbucm.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gqwxwmuye.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gysueqzma.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwbdkcaqc.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/grdhzrcdr.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gpdcxxafz.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gmixaptto.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/geazecvcf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gbdkcnasm.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gvnwepatp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gsovohwyq.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gxypokxmk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/ghegeqyjh.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/ghffumllj.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/grbmkupic.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/glonisgft.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gheqsbyyr.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gutldvejr.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/glbfsfnlk.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gvcbmqzps.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gvtmhsasm.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/ghkqdjweb.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gdfgunwtm.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gugirifhy.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gxfolaagt.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gkuwflpoi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gkhdstbor.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/ggxfsymas.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gnwuqltxz.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gfsqwjlgu.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gtwpevrys.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gpjtdbkot.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/grynimrem.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gqevsrzql.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gznqfnkwl.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gordzclyp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gbbvrbkoy.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gddfiynrk.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gisqefwhc.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gcueavnij.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gkfcpklkp.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gsevcfpes.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gomtzdgci.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gpojejxuf.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gtyiptbqr.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gnkxgwtku.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gkqrcewhg.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gjcxykimo.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gztqpqlic.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gwxwodvmq.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gevoesgtk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gfjrofjmh.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/ghbysjwud.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gdsvkzcbc.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gfntzmsul.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/glhjwumxk.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/guhuvlfxp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/ghyrysamv.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gbwjposjq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gqrokdjcz.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/ggvgduebr.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gnxyrlavb.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gbnesvouj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gwgghdhwf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/genfrqdrj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gmmhlsulv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gslhxkulw.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gzuoubwqy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gapihtncf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gxlvxttgq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gwzqyyxgf.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gilovoazy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gshlodjei.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gaayimzej.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/ggavnshro.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/ghvfkfkwe.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gizffyvlh.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gldztlwjt.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gjkuyavuz.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gapwxreth.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gdrnjvman.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gyjbuptjq.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gjzgbmxvw.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gkwmouonl.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gvaiiwgyu.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/glesiapqd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gxmmhyzgc.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gnydfjheb.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gjoxvgspy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gsggcuuht.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gaidutbdu.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gezdsaghb.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjixpxuv.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gpqzfdjqd.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gztvqgygj.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gvsgmioew.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gedzbilfp.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gifokgprq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gwajjueid.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/ghrhddngd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gnkgayxww.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gkxpqdqfa.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gvtzwjsun.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/giswuvcmj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gredcwpop.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gbldzdzqi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/ggqlfegow.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gsftykzlr.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/glenysrku.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gsoxfauna.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gcuqmfyqz.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/grenuinxt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gtakkbajt.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gsgdzmpiz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gjxtwmpid.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gdpdbydqh.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/geiowcxjs.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gunhrtvec.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gnlkkjfeb.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gdhgosboj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gjcbzpypz.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gxrqxhbaf.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/grqmszruj.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gmohhpbgl.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gwktqamal.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gqmfrodgb.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gouefmiwb.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gskumzbyq.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/ggweeqmdm.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gychtxnqt.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gothvjjch.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gqnqnfklk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gyrcepffz.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gfiovuwgy.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/glaafxjqg.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gayrqzhmr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gnvqfdmei.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gywwwucgh.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gwlriuxku.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gcyyehwjh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gitarupwz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gexdrznkt.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gjpekpelo.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gebxwcifl.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gfqvxvhqk.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gndmejlwn.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gvlvagpio.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gnmokucod.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gezoctvcc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gayviegin.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gnnkwbfxe.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gextslklp.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/ghuzmcqax.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gudxmicby.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gmsodtixv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gddswmpfw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gadcsipnn.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gccdznubt.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gzulbfvvd.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gdmmzsssi.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gczytbnbb.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gzvttqscd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gsfjcqaeg.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gsdhtzkwy.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gzyocoaud.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/gnxnifrkv.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gksgphrqv.sHtML


<!-- 参考信息 -->