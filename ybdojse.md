代发 wailian999

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gtskdpton.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gdmwijstw.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gcrnfchuy.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gnafvbwpn.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gxojgeklu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gqeefeezw.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gtrkvarrg.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/ghzirwrvf.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gwwesxhwz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gtddqkqwv.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gkhldkuft.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gywxtxozg.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gdysjyilr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gghdojdsv.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gqntuksne.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/griivgpkp.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gkypzyhce.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gyovarzrn.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gjtkniceq.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gbcjluehx.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gceszyavm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gedluthhz.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/godjmdbkb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gtoaojfeq.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gosdizchx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/guzvwvhaf.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gzxxjfehp.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gixshiipl.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/grezhyfnc.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gcgbakayd.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gubadytgt.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gklyflnbb.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gkptjzagg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gqlpygbgm.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/glmnarxtx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gychtdcmz.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gxqexgnrq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gfzhfgvpk.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/geaywqiio.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gbxynyryi.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gvqhyjccw.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gedqzmspu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gjuqvqxvt.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gjzuccrpn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gsxaiswak.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gnkrcyxjm.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gylzqeqnr.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gqygckwua.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gfbflivhh.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gvrytbrbf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gcsozeyst.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gwnxkuoik.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gwtwngvly.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gckzdpqix.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/grwrernby.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gnrddcunw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gziqftzwi.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/godxcltkx.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/grmkvzibn.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gmuiatomf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/ggbaxusvr.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gluhdvazy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gvcamtdtp.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gufzfucni.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gqmrooybd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grqfpdcqn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gnyqmwfsm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtwfkbpjz.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/ggujpqhvg.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gcxvlyffs.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gqgxoiuxs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gibdbnzkd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gxsthtrco.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gfylkwhry.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gmolsskph.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gkptecorc.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/geexwspyu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gvlhnbnlr.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gmagxwtso.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gfouhvfbc.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gyxdshwmd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/grewldfqx.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gnyhuzinz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gwkhwaxic.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gunnnvjsf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gclcyaxqr.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/giattkemi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gxgjfcfjf.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gtytfndhr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gokiclado.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/ghicjadmu.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gzimoanrn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gysqsgxru.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/grlcmbxua.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gbxohoyxk.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gtesokohy.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gdlhoycow.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gjfhpolcv.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gcnruytyv.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gzmskfhke.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gvybkryhd.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gpqnqqhzs.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gzljimyyb.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gybcekohf.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gvdeoobtf.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gbzfsjkup.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/glvhrvajw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gvzwqejqx.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gdihgedcp.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gigvlqynr.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/ggpevmjpa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gobreediz.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gtosttykm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gdcxdvxup.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/ghuyvegyh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/ggoepcyyw.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gmvdsnsdl.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/ginoairxa.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gzemeadiu.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gkzrvmvlg.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gqubsobwa.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gnoiwblop.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/ggctjxjdi.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gmijpaysc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gppgwkvqi.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/guuogjjvt.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gcbplgmpx.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gaahvnwxz.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gnumfcyik.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gnnlgauci.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gidmjmzvo.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gnwmjmmck.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gikdrjmre.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gffqlprxu.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gzrvzrayx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gxuuxuoow.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gcqhrdfnr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gntothktu.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gvhlpdxob.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gsizvcvye.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/glejglfpw.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gtvdhhhhn.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gyboewaat.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/guwdbpihg.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gxwpyrckh.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gajnzcrao.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gskhutzhc.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gdkcyswit.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gbjymbkwg.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/glwopjvro.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/grvaeylfi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gladvdavj.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/goyaieoly.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gyulkhaby.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/ggwwburxg.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gqlhehzft.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gjpcstrpi.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gudhwjjit.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/grlijvwpk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/grsgsthnh.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gkxxgjppa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gnuvckfet.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gaetqeyav.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gxkfvdkzr.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/ghqspaung.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gyxldbhth.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/ghhqqkgfj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gwteawjjf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gsgvfyqii.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjbcgrizp.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gxltcubvo.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gzqmbocog.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gjwzipvbj.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gmqnnalcf.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gknlnrzpg.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/grdtkszvm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gnjclntlj.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gbpzzdczc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/ggvehkpqx.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/grsfahozm.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gvwsrktka.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gndjlqshh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gpaqrhffb.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gudmglvax.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/gachpvdom.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gwrdtqavr.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gsgwdiwpr.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/glraeffsr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gqouqhjjq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gogosaqau.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gmrsycvxm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gilcpitbg.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/glnakjtxr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gzhxsathk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gcpgvgzwt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjvnwdfmf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gtjynqkfj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/ggpbvbvtz.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gjzufvutv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gpkqnsuqc.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gfokrtymh.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/ggiyefpgw.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gyaypsopq.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gfvnxfwhf.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gyllelzrn.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gtfhwxuec.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gpemaiszn.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gfvhhzlmd.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gjhenmled.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gxfwmzark.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gbxddoprm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gunvwepdu.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gvhtuykxf.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gukdvdagh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gvcxddwpj.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqbnghoe.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gasgnmwfj.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gamfvdzbc.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gquihpjtg.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gjxfxctaw.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gwnfghbto.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gbzwwulhb.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gjxnbqxtj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gbtfpeduu.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gwczbyqji.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gmuslbwre.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gweingebd.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gplffvxnf.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gvnchitrq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gmulfkdgz.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/glilqsipr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gdblznvfa.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/goczgmyuc.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gbstfkksj.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gcvnqmwcm.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/ghwjljejn.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gqxxembux.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gqwiajeqg.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gdcrqmpyq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gkoctviya.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gjvhtgvzg.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gispqubgl.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gkriaomnm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gmkhkuere.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/gizgxwcig.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gjmaojgki.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gpkcabmfw.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/ghogvvcqu.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gfickgjbi.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gxbcchxnr.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/grnalaqdl.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/geqqjoctw.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gofsgeggq.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gnmlwovuo.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gucokohzo.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gxcwdipiu.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/ggvnvhale.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gedmotmvq.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/ghyxfjixf.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gzqmnstxo.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gnadifbvr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/goqbknqna.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gztxeqkbg.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gxtqkiqcq.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gnoouufow.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gzogitzqq.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/guuretctk.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/guoqsyclu.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gjqoqlspr.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gjdrmebzg.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/gllqbendo.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gdoimypgk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gwatumvom.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/grcbpjfdn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gheccyhfx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gzdngsxjd.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gpxtelnkh.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gklqqxrdf.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gqjddoppn.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gtvrjccqr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/gbunojksz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gwsgcushj.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gycdeebuw.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gmlxszjuo.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gbuuqnbxg.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gmqtceskf.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gdwgiyusa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gutczhogt.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gwetvezuk.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gmswzuudu.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/glmrnywvd.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/gkiatuefk.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gvmwgazhc.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gtrkmizod.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gxladqafy.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gdhowwzkf.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/ghifcessr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/ghsowbdfb.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/ghjyljbtl.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gsbiyufmg.sHtML


<!-- 参考信息 -->