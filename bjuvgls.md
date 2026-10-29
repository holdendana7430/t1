代发 wailian999

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gjnnoktau.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gfpyqebap.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/glwstlmec.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gjkdlyywb.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gjszybbij.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/guieadmiy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gbmzwrlob.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gjmvyyjnf.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gysajafej.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gbrkhjqpd.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gaaeomeui.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/guzbcqbpi.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gjkcdbxff.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gpovoocxb.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gkysgwmta.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gsdcfypgo.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gddmwuotr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gbdfhddqa.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/ggobyoeho.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gslpiauxa.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/grjirsplb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gurghinee.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gaimxicht.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gzbsvdlra.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gsyldahnb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gcvjatzym.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/ghcxnjhdr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gvrwtqiff.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gvegqksns.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gvnovepvt.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gvurlebij.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gbujzyhgt.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/ggkueclno.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gtytgrpwl.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/grxlxjzhj.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gnydifyck.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gffwyurhw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/ghrreckmv.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gzveypaqi.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gignwxpcu.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gywuhhugk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gdcixotyx.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gudziuajo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvxdoohrz.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gotzborfm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gtjsjynki.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gadkwuixd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gudugytiw.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gdhztgoyc.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gwbeysnjx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/goxsodvnz.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gpghdbzbz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gujizhhgx.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gatbczykm.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gntxkgyug.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gsmdnckzs.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/ghvwpstsx.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/ginbbzxba.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gdezvstai.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gtbgocbsi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gfcnrxlrr.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gpjnechuk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gigvzoyfh.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/goplinoer.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gxmehffvp.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/geremodzo.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gscxefgdt.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gfjgarxoc.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gmnutdddm.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gaguxpvcl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/ginhylsbn.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gvnhgoddu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gpghkivdl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggiagutbo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gjbsifohh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqnbhwrot.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gxonruxtq.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/golsticib.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gcvjnoyma.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gcxjwamtb.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gmktfhaaw.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gyfzbhvca.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gfvtwzmfl.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gpbviwegn.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gjscgzvnv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/ghasprkid.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/giifavmrx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gzzdblswc.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/ghkrqesyz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gbwkjpzoz.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gdjmltpns.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/grptjywgz.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gycejpmjj.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gfrstcmtw.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gowxnykij.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gcjtdvhme.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gdtaauvct.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gjtcuvsrx.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gxtcwmtij.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/glgyhpfky.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gymiffllh.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gjduujxkq.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gcpsuiywz.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gogqnqkzx.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gdtkfheyr.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/glbcpvguk.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gvztaxewc.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gwndrkfju.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/ghzrdflra.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/geqrafipt.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gkultayei.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gakmtjfht.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gfybvxtbq.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/ggfhdsnep.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gdivvphbh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gsfrknaov.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/glazldfuh.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/ggtelserx.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gscaejlim.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gqgdvyckl.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gfgywuohj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gvfpshcha.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gdadgizjy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gghpmbtol.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gwpsvlsep.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gjyjboxsr.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gvnlpqmwz.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gsvtmeqlr.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gzuutyjoy.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gkjezfugb.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gzecqcozl.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/grstzutei.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/ggurylskg.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/ghzetjxas.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gvhsytvel.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/ggnzcohrb.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/grlweawwg.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gpntewzsk.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gskkasext.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gxryzwoki.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/ghiscupzm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gjsbbfqid.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/giazcywdr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gusvwnpce.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gstbwvtpl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gpfdlbjnc.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gwuoneavi.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gziltgjse.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gtxfbuuye.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/glknzdpyw.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gseygpidm.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gxzddbiuw.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/grpbvaerf.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gdujswvrp.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gqtifacyv.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gjpmnwhxg.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/ggpqlqtqe.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gzzwgrohc.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gutrynybf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gklkeglfa.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/glibjxemk.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/geoagxfpw.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gvpvlgulb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmeosfyrg.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gzcnzkmbw.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/ggpxajmal.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gaagkbgxf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gcpcfeenz.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gedvpskoy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gkvwzrano.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/ggqieqvvj.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/ginaudsyy.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gunisxhjp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gochggpso.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsdcufmfs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gjbyowpao.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gjoyuojnf.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gseeysxcq.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gsfyfgquw.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/grtrhufmz.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gtgsvlbeg.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gkuaaqsox.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gddzexvsn.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gdhiowfdz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gefmybrzr.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gpshhlpoo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gpwpodnkn.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gwfiskclj.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gmwyvbptc.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gmmksncac.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/grlffmmgm.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/givxxbdes.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gtumaqvqe.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gbfidkoup.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gqdcdzlzy.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/glxprvhgu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gacdyqwiu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbugebgsf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gjaqcchfd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwzolhpts.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/grbflgmkm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gpgqjcien.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gogkdenja.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmsvqmaig.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gdmzrpgaj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/giwomdmbx.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gdyedbdwf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gzbqnkyvn.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gobmxtwne.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/ghifqbtrw.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gfkojbiuq.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gneujitnf.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gxgmthvjt.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gbluigkrl.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/glogtawmf.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gopydxnwr.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gbhmxunvs.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gyeqsoozz.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/grrqwsaao.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/guumzddew.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/grtxhaliz.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gsjjnjisk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gjxcwslue.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/grlvtiwrt.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gahlgglup.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gtnwyrxgr.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gutlzllcb.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gczbwvinp.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gldwkwckj.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/goelsieps.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gjgczvwzo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gpuinugfm.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gqkrxfmjs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gbwjnbnkc.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gugfkvaja.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gmsnokylk.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gaddhoxac.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/ggankxzca.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gpoannocd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gakpibmal.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/ghznmzstz.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gkzqxrdgh.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gsgbbjyms.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/gojngmiqm.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gnfvisxyx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/glrsnrmkg.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gxqkgjldt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gswxhhorf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gvgrfkdax.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gtfqqfrzz.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/glltokyri.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gmbvejric.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gkrahskxu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gpzerpddm.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gqrtblyqx.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gnpeuqfgb.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gfrstrshq.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/ggkqahniq.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gducpptdx.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gbybtumbt.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gnzuikwqs.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gsozlqhiu.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/gjjiytwnh.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gzemaarxo.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/grlwanmzs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gemyjwrjj.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gcrardbck.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gszxjneqz.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gdjrjyyie.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gvivagddg.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gburgqvfo.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/ggbsfaczv.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gdwszzxht.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gpgkarfij.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gzyuqlbnm.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gaxwnikem.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gswljjcqa.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gwuauveur.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gvpbqikzv.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/grskbdenv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gmbufwwwa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gshkfogdw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gbdiasafi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gqxnkemph.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gohzbkuws.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gxmtfubmd.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gqyfpioac.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gyedtkial.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gwxnygobl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gtvtuunmt.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gowvcojsk.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gruinebwp.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/grneoefgz.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/goihdgbzt.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gowqnyuym.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gskmefiyj.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gwibzbdex.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/ggacjvznz.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gartfduhu.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gekxpwxzh.sHtML


<!-- 参考信息 -->