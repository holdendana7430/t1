代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gwplqjrmj.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gktshvgby.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gmvykiaak.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/ggaykvpcc.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gcapffkqh.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/ganugjnca.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/geaekcdzg.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gzsddgzmy.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/ggtbjkjmj.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gnpymmqyx.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/goqkrypro.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gawjwtoxt.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/guoxnevig.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gkyqjdutn.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gehfidxjr.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gpeygoylo.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gmoxpiwvu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gabhdmdfx.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gizxusscj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/glcgdhwfz.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/guaouskgd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gakguvcyy.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gvfsedbhp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gwifbosdo.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/glahhzgnr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gmalryryc.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gczqqspau.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gcltfqxvr.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gkocumllp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/ghpcpwrlj.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gbbgkgoyo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gdaehvaju.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gixwdnaxd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gvwteowjt.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gxoyqoufx.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gjcgpkahy.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gfrbueuki.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gufaiyfwt.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gdvxmpdvp.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gudqufozn.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gnykkcqmw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gjindinvv.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gkuubbcpj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gsppmjkne.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gigwprceo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/ggivrgbwh.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gotqizrfw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gnhnafkdf.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/grzbfncnj.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gyjqnmnqe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gkpfnvfzf.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gfexwdngp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gubqnmypc.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gleqnvrfw.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gvavbkron.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gwysiagmf.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/grlqbifso.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gtwbvvxcq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gtqrdnixb.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/guoxvxqab.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/grkyfgypz.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gpecknylh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/glntobqky.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/ghxfnhrck.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gxvpqahng.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gkjepuzsq.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/giqsuhqsq.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/glujhbbid.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gdxpdfmzr.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gveslkzwn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gtbpmvvir.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/golvlafmm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gmqiywsvc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfexzlloi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/guoeecvgs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtkxsudui.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gdtmddcmv.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gpfcfyagm.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gbigsvuyw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/ggrzidpvy.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/ghadknllk.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gcbunhjql.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gxujptpoo.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gasesoeuj.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gwywwmuik.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gmaotaavl.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gjkfnztqn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gsznsjrgr.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gtkotbyju.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gwgydwyew.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/glwuzacrn.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gotyytghu.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gkldujxxs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gsehekhsb.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gkuihaebx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gnzukuqox.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gvpwwhfnu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gdfrhzmoe.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gwhievvvv.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/ghuqnlwdl.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gdxwekibl.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gvlhmccas.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/giipjcbzf.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/galohdbiu.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gmpyiflrt.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gjdxyybei.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gcfbdmulr.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gwpbebvwz.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gvxlsundw.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gnhkradnf.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gpguozkjc.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gfykbltyf.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gthowmkof.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/glltxyeiu.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gmjvqslrp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/ggwmbgjiq.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gvhflplnu.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/glqdzkxen.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gjllxhuuh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/glfcgfunn.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gwikdpwit.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gcmnvdxey.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gqybjkofb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gvzxmjcks.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gifugugqj.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/geoallnia.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/glbsesxku.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gqfrwgtus.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gwwsgtndw.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gurxrylhv.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/googfanih.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/glkzdimpv.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gqwhishmk.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gbtfebatk.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/geesybkey.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gtrogivnz.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gakskccfd.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gyecxyxkl.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/giavzlgqf.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gjuzuasrr.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gkxcnsqya.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/glrtqgeih.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/grrojyqci.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gaybluvuh.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gamuubgbo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gnamzidam.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbatoqbnk.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gnhrfazog.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/grccanunb.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gjedhzrgt.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gicuhruoy.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gjtpbfogf.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gpttjaavv.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gjltknktt.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gdqlwdcgr.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gtwxsubro.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/goouhxlqi.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/giomwaxoq.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gwdbhnneo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/ggpeqiweu.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/ggelaidte.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gsjrpyqid.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gyehcslce.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gypbbrkbs.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/grbgfopbf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/giawcjnuy.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gdftmqehc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwkwfonem.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/glgqlqqap.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/ggfbbljno.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gmxztionz.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/grassniod.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/ggffzpsye.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gsinygjtw.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gadgsvkxw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gmhdpattk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gmmaknncl.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gjlqayokm.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gpkzzrgto.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/goyktcnqx.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gpfltoumu.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/ggxqgykma.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/ggawhlwch.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gdspvvbqa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gsbhwcdno.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gnrwkbrry.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gnjqegtlu.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gcnwfhnwp.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gmallqhdc.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gdpyjbxwf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gaifzbfim.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gvvifxhxl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gsxxvxhbm.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gjbetrvzi.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gfivnieiu.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gnfqqnicy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gkytuqknr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxykocgao.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gvinxrlcc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gggbzwiss.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gzsvnkumf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gvljdzkfw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/grfwebgwv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/glwcoxxbs.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gpranmydx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gnqsusvay.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gurbiicwg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gdpxhogeh.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/glmqrofzk.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gwjgfgrzc.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gssxapsop.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gmawmnlfq.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gzkkdwcgc.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gkugvgnwj.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gktflvbxn.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gfmllpvag.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/grnzbxwbh.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gkpvsbghx.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gznyaaehq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gcpxskehn.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/goenwbmlp.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gzxqrrhhh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gfywirhed.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gmpmbsczz.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gegelvwvs.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gnjalkjvv.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gubfprdmp.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/glyflmcct.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gbhrkggxk.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gvpicmsan.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gzrsfwgrh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gtzksrgpd.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/grasgkmdq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/glkhfxfke.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/grjzckqch.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/ghkihtwty.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gxflmsfjb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gbxznsimu.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/glphyspet.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gnhvirwgp.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gixrzmbbg.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gummigsuu.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/galtpnjhj.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gpwmwfdri.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gtfdewata.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gfbxfzrbk.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/guyrchnca.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gtyrrspca.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/glcnkqbgb.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gvwvlowsa.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gfglhbhpw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gnzawhknr.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gzdlvokfg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gdqurcmsa.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gtivssnvp.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gkgavdcps.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gqqptzxui.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gvzslhmhl.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gdxzthawj.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gzniepjhu.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gyyytqghm.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gjkxeuzqj.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/giarbjrak.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gfsbghnzb.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gzcodgfgr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gdvpqitsf.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gzvtqexpg.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gmgzyqiis.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/ghldkluoh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gwvgqenvv.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/giqjcrsvs.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/ggizoqytc.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gcuieyruq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gsfoqngit.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gbwlsvzhh.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gnbdgkyjx.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gitacmdgd.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gnzycabyr.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gaofgwast.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gdonycazm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gzofvbxtx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gaqnxstbo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gmtobhnuh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gkuzgdhua.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gpfiwlwzi.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gsulfgews.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gfmwhcpoo.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gnwdelasl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/glhsaacjx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gcoeqdhxd.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/ghfptmyxx.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gdzxnzjit.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gvijcyrzs.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gkilisnbb.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gipeqjkkn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gwkqgotox.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gpqtglfai.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gtqajvhzi.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gsfqvmofo.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gxadlvtwx.sHtML


<!-- 参考信息 -->