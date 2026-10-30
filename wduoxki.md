代发 wailian999

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gqqykjvwx.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhbxinpc.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gdfifyury.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genykgzrv.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzckwmut.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxtxqdzzp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gcrxnngci.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gqpxwuagg.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbxumbwe.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipnnhucq.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpdzwrvd.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gbzzkbchk.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxiwjesa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdkuhmiuw.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcgmbyal.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/guxndgdpj.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqweurit.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacbbzpce.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gdztcpzfw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpyuxpuol.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gjidbbcmz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gifzarwuz.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gzyjoslut.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaqemgvf.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/ggugxzlnq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/glszyuczy.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpyjajsy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gackhupqt.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gypkmhmsj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffvyyrjj.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gwgswwati.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gebtvuwmn.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkyucqswf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gynnsbzki.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdfvrjmva.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsjgsczp.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gizlusuui.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsbprkjk.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/giazoviou.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsocjoeyo.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gybafxjqc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhocyvuh.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gbodifzqc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbgvfsivj.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gagudhxcd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkkckupg.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqocghggi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/ggmnklcwm.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gofejtkup.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwiuyjpff.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gmopbyopp.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gdsseytmz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/garkliwdy.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gvrcuiveh.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/guddhodnv.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gdymqzahx.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqujsaebl.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcfzoufw.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkowqahoi.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gnovwylzg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnedbymlv.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gipvhxhwr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyxzymvp.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnpwrpgo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadrqiubx.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gqogsuoug.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbzexfrb.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxfdpufh.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxwqgqvc.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gafgtyjpl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gmxqaqqoz.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlifkaju.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gvslbpejl.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkodfnvcr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmloixrt.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxptgxzqd.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtweonky.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/grtmpzkhk.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqbyaqufo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsbbqaei.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gaudacnal.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gzmkqntbd.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gpksgkuiy.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnwcawsd.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/ggojivadd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/girvxlgkp.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyfcwclc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnzslwlg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gvehzjqcg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbosgjvdu.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gtsepqptu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvanzzchx.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/grulivrfw.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gxftdjgkk.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gigxbnrjp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdghhyjt.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gszxqugwq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gurwktzhb.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbdjplfv.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxygzqjmv.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqiitxif.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwdochza.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gxwgsxwzv.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gdnafueor.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrfbdxqy.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gqitljplh.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/guawtajci.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbavmqga.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjokcmmg.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbkgvdul.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvsbttuw.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goklnqmrh.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqylhodz.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gzpmkbbhc.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/goigevcyz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/grmbjgfoi.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gvowmeqkk.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzlvuiav.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gyqtrpafk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gzphgivin.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjhthexn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfxvatoj.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gukoelpze.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gewzavgtl.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gzesvqjvu.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gldhxtbcs.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxrrrggj.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gosvholfn.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxwyedla.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghijlasmr.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhnxjosc.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gwucoizjj.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gprqrljwe.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwiawxmb.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfgjxiee.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaxgpyrr.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gpelahkiz.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gssisblkp.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gsdmzmbza.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnforzqr.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gybtgqaen.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gmrcnfitr.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gcyuprmhx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmddxyoqd.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gneqmhptq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauptthhr.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gputistao.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gmrdggndp.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/geurbkdbp.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gwyeygsou.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/grxgexfvg.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/goycpxjqk.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtqedkqb.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/giwlrytlr.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxrisfop.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gmxdlovfn.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbgtnhqo.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuovkkts.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpbphubp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gtngrteug.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlyjtybo.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqiqcvtk.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gzxwqzitc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdxawkrq.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gexmruiua.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbzuzvfr.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gbjpyzgzh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqplcqpp.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcgfrfdm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gonmrdulm.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gghttikuj.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgcsnboc.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwrkctmec.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnutpmkkv.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gisflachl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gvyismubq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gonxdubwr.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gshiryflu.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gweejwxpl.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gsppdtkuy.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gestixzzp.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmotkwuk.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrwgpnba.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gozcvnjvt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gggwgjtzw.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwkzvyvn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gjcdsohkw.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupiwjseg.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkldwkbzj.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimnnbdvf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/giwnpuhad.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gafwdxznr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfugucbq.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnlithdx.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gtslgzvbv.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gtftpqbuv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/glhmvxkub.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gahoytcnb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gqaxhchjx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqysfxedm.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gcyjmttrp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoxkjxnx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxomrmzx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtjrznrq.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwdjrrno.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/greddmrot.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gldrirfpn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvucwmep.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gxxhofvoq.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gakoyofub.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrbzvlnx.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrjxyhyq.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gfgkinqnt.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gllbynask.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmavjyoc.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfmovfxu.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gwtiwxkbb.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gzofcibbc.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gttblvtko.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/graowxplt.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gxbusqgtb.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgxijhsy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrhaxiyc.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmxfqrvq.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gbnnfdimc.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gqpvoipko.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjxkjzes.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggynllwou.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpuvzwjt.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpcsygqz.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/goxrriumm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvkpznjg.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahovpjub.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkmdjnao.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gjozxoqcs.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gffgqoawp.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gjnrgndpo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gqdvdpjkv.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gyovzbovo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzkquare.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gdoknkbmq.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/gibelxehi.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gcvsnoxsa.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/garxcqkxd.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojagwbey.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrdamxuz.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gmztljygp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzawsjwq.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gkyxesows.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkejpiiun.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhwlcmxe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/ghyrqtemn.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gwxycoogr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gpuaiuqbt.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/gbqbdvyjg.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gptpsicif.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gmalmzxmm.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gryluzxhw.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gqpyvozbj.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzsiqdiy.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghykilffz.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gdufhrsoc.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/grhqtgozg.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeynfqbc.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/goyajkmlw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkanimog.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gaichsdeh.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gypwdtzyq.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiazfblv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gibfmhppi.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwtcrkhv.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gwvlbifhe.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgawptce.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gbefxlipn.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gsctfuvod.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gikptniqp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbmxkped.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gqxvdfpac.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcsetlrr.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gljjgdygc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gliaggnae.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fanxiaobao.xyz/Article/details/gzrawjpjf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbwtvnit.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gmvcuwbgr.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvdnfefo.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfrbscmd.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gkgniphqa.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gvsxwwvhz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqgzkjqu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gldttfwcl.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgooeogi.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaukknor.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqnixnzl.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gcapgtlet.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfjqkpzt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/guxwxtntb.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzqmalzm.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gjipnlnis.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/goacjejih.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlmydqxa.sHtML


<!-- 参考信息 -->