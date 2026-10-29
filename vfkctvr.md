代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/getglrpwm.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/grpdqicek.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gyxeojibi.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gnljittdg.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gqdqkedsl.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gvaedhyzo.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gicdlejvv.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gwdugwjit.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gnbgmtaiu.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gsrjukckz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/giomtdcqn.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/ggrvwmrqa.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/ggnsgbtel.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gljrqlawr.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gltnfqaom.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/guxwfudgi.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gsnhekiwl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gydzlbwmt.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gxbmskery.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gsfhlwnkl.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gckblysek.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gxmbrakhw.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gmfmkwmel.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gpfpgzcyf.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gyujgieta.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/goyrwpavi.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gsckyfkvy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/glwjkgqet.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gfzfpzlls.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gerpczepc.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gxhxmdvfh.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gpuaypeum.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gapggjlxa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/glwbtxpys.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gaydpcwpv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/glbdismoi.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gtaswofbv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gvyvhmyle.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/ghfpkmlfz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gcvkwbsqm.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gqumedzex.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/geghxktkc.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gxdqmimmh.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gglqbjcuy.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gtvsirmob.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gdmxyxqxx.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gcvttgpxf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gjrspuoma.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gplannpsy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gcxmvudkf.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gpckyztmb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gqddrjwok.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gpmboezoi.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gbkortidu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/ggpepvees.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gpiyepsef.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gfjhekwyt.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gisfzayjl.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gkpmlymdj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gwckraiws.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gricjyapl.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gktttokqm.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gfwlomtqi.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/ggugfznui.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gqovqrrmw.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gklyduvhz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gnvpujmbx.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gtgjcywqf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gofgvdxup.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gcqpzuedc.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gzpomhogy.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/ggqhmevpk.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gemhfpojr.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/glenvtald.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/grlygvikz.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gajrszxcf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gvqdoqajt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grjdzsqbz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/ghoiizgly.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmrzhjszv.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gwacngpbe.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gllshvefr.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/grugvideo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gduxlquky.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/grtvjlddx.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gsltpdktq.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gvsgmbocq.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/godcwmduk.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gxflnnaln.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/guhxkcrsd.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gylfoenmr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gijtknhps.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gosqjybnb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gukaxfhiv.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gimrqfkyc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/goacewmzm.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gkwosytzb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gmaejmwjn.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gkersibzf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gnundhkpa.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gxekaunqi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gjmxvwbua.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/grvrgpnml.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gciumovsu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gfgpghoda.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gxqtjngwh.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gepeztbnw.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gnufhnhzf.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gjcakebge.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gxtowcggb.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gqeizsvqb.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gktwyhwlf.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gtejwxrmx.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gncnyjjmk.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gfpiowuzv.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gblajdmcc.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/glcmqudmr.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gmqfnnxim.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/glgxackvi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gccpndqbv.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gpyrdjkbb.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gclmrfcqw.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gknggyvvt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gfnnlhies.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gyecpmryp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gbwmsfjcl.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gfeqoprtf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gfqyqfbbh.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gmdrnzrzu.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gfjuqhyyn.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gwlwwalge.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gobvahrlo.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gnspkbabc.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/glfzjtewh.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gsecqmimn.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gjsnytxbr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gztzkldue.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gmwgqrdyq.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gytepdgtq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gkyandxxg.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gegrhndpb.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gieizvnrb.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gbxztnhth.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gshvrxfhx.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gyrlyqbbh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gddfcntdp.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gkstfrmxc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/grltjysvd.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gzqqsemax.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/guviobdeg.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gzbgqdfyl.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/ggvsouepv.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gigyirmtt.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gwpigwyxs.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gwcqcpyqc.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gocyuztod.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gkuwqbdfp.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/guostfqxo.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gbupntqeo.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gwuatafku.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gasfqinix.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gppyvtftv.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gbtwiblrj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gfhnmgcuy.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gncmhhgpn.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gmcqhsgsg.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gfhdgdcdm.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gcsfetusd.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gtawvmbho.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gxeaixfwn.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/givkszdcm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gfjnjfryj.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gozazeseo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gkrgnjfxl.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gkmlqjzjs.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gpwvhukvq.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gtpjwwgpz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/ghppkxmva.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gqnhgpnxq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gvpducrcm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gwrmefjzo.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gxldhktsf.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gearavbpg.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gnocthrca.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gvhvtbene.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gaadinewg.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gfutvuurx.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gzzppulrm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gjpsrehbd.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gzefhrhtw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gvgsejtsp.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gnnjgamdi.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gpvavwcri.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gdyqpavpp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/geegpveay.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gnpuepepn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gpunvpywc.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gsszeeexc.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gytzqmapq.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gdxommack.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gnkikfjrd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcswuxdaq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxesdanen.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gftlwthyy.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gybdsiqhi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/goerpehzm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gxwnrqsxu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/glsstbrdu.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gypbrnnuo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gnsterjlp.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gearhthdf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gpwwpgjeo.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gjqybomxl.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gabocgimp.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gvpjyrfvc.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gzduvcgtl.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/granilzlj.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gqikgctdd.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gmjrpxgal.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gpzxlsolp.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gnqewtvle.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gqqjdgtcw.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gfzeodjqe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/glfebnaif.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/geumjuohy.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/ggggzkxoi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gquzptbsy.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gsdryszqs.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gpekcopol.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gxccueeir.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gwgricslp.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gmuagncai.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gnwswanai.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gncpoxbhk.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/grctwdbmj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gpptfawyt.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gqwtpunmp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gidqbclno.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gqwyhlbjm.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gcmjkgrbg.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gusguxxdx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/guobtjiho.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gjcamkwpq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhzhbxea.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gbkgydovp.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gzqmjctmb.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gpyjxxacy.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gwanugbeb.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gjbzalbfr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/ggqdgegou.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gmckowgsv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/getoqgtnm.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/goctnshqk.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/ggmjkjubb.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gjhzpqdzr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gwcqarotz.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gchfnvsxg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gpyaoexra.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gbqkivqad.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/ggwkkmysi.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gywyvytfz.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/guzmqtpuh.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/grrgjaxci.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gxsmbxxde.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gurnhotuz.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gzqglgasp.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gecpireul.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gxzxqmosn.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gwielohat.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/ggamdtzxl.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gnxncrkwt.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gruqjkjcz.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gmaxyjrsx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gfgioiubx.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gltxxlwce.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/glxrjxtbl.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gritcojio.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/grdkefodc.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gkkzampci.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/giteodxhz.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gjohmoruz.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gduplnxxd.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gfubeuojc.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/ggkjgfnye.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gmregvyhn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gbozeksmo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gsxrbvmqa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gkeireuan.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/geooemtkj.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gqqlbcxjm.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gjzmflzhs.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gkxjbyyuz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gcwvlljqd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gphoxtubr.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gwfwysksc.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gbjwuufmd.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gcwatwirb.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gqhgyxlwq.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gxluvheuf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gicwqkumr.sHtML


<!-- 参考信息 -->