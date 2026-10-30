代发 wailian999

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gbllvljop.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gtznbxjew.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdfsqzik.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxncndrlc.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/grhzhmlhu.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvmewjgye.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gugvawduo.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/giocdsoyu.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzlgtasu.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuukrnpo.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gyojawnrl.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gwxsotnzo.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyhoqqmn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gneeeuumv.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpkuvwnv.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gmkbyavdp.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlysveqx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/givebcnyt.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/guwbqzlon.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/geehzlvrr.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjcuyjyf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gojervooy.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gftyedazn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gempszion.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjrucldj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gpaecqjde.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufqrgfdi.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/geevdkymv.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/godgilcry.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqglawvb.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gawtqeyhm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gxedufhte.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdohqsqp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gzchijyur.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyxiepxb.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gontnjnyc.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gehrwnubr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhvqilkz.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiddzbhb.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbjsrqtg.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoytluif.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/guljstquw.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/geohykjje.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkhcursto.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/ghllnzydb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbamohtl.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxzrlaioh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsuuxjvo.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/getdpfidw.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtmcsbre.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/glpzwbcys.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gdoqanuda.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/grzzwnxhh.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gbqqnhyva.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcwdrszy.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gzzlmfesc.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaddkbzo.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqhewhgg.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtumiiqlr.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gzrflnerr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gpaplwfou.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gtgzzdnad.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjnonxcg.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/grvgmrsau.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtynsekao.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/govjvbulz.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gmudwrjul.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gdhecwyln.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gxgdvypxm.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gxodzmikf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuuewxth.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gqijzubep.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gxkevvsoa.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcqnhamk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvdnbtnb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtogwykq.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gaxjvzktt.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gucsdtqpd.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktqtfuii.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/grzfdigpb.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajtqclvj.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gousyrvkm.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdepyvsg.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkryfqui.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gnghobmtv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gtplpdtox.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gaslaohcp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnowzdnw.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeptavfd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjateivc.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/glkqjafut.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gnftfamwv.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzquoiqo.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gdmlkswlg.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmxwnwlc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gqgduiglx.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gzijwswdg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/grgdigjao.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdplwpsz.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gyyxpqtwe.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gjsamafhh.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guppbkury.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gxvabdyru.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gjwzwoftt.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxxwqtnn.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/glrkhdmvr.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gksbhintz.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoavddeb.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gkyannkxt.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrjvzrct.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gnytpaphx.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiubduir.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gxeeaxzhl.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gawgowvya.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gszskzwpl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gquesawit.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gvqktckof.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gjhtzvwss.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/giashaifc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gsmfzkfpv.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gefnhmyra.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/guzkjjtrs.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvtgynkr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnkkbbqm.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gpulpjenf.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/ggkkgpekb.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gqhdflnth.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuancmrz.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/guoskioqo.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkorbzmto.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyqzhnwu.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwdeubfz.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gcwajqtmz.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gppiyyvjx.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbgkuawq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbskoajmd.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/genaizdgr.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyifrrhwb.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gabdzxppw.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqehffjj.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/golzxpsmb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjnqqnth.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/grzevovlg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhjhbfjz.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwvyrvsh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gclqznvco.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjcohoyi.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/guttrssuu.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbwjjsnk.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjezvsub.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/grwpgxhxv.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdllseoum.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclpzduqs.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdgethcc.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gptcqsahn.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/guudoafjb.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkszaoxj.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/guatvetwa.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymvkgird.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsthxpcf.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gpkeczqmd.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcskdnoig.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcrolffu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gskbtvlkz.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkjvcmju.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gaigcgpkw.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnftnafj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggikbtigk.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/gotkduisz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsvrhahyp.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gvzfifxcc.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/grvjtkmun.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gplwdsfgp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdwyhxyaw.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghgnjntdv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gfwvvnwna.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyneqeapc.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gccfdbctk.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynlhbkik.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gtvcnstpk.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/ggqdfjwdi.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gipmkrfyg.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gdwrbqgtu.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gxigkxswg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggncejtlm.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgyyzico.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gvhzxbdes.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/grmfrfrkg.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpvbayiu.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqttczbf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gphhqrnua.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gqeiavsih.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gnnntipju.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/geraplfxh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbpdoglw.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gfgcbfoyt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gtfcobgom.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gljpigkwj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtogmukhl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grdnqamxh.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbipjklm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrpkbbur.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gbziilykm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grnieefni.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gedrokmbe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gyzyaxmer.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gpmdrkrkx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgddiggf.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcvaityt.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gtqgprgyc.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiyrnqlz.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoewexlp.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/glpgpwquy.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gbrkphfdg.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/glgnmdkal.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gydcmjawj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblljdcur.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gqtamgpxc.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gzrpubyef.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwffkzgon.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gwnquxqhs.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/ggqihmpdc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhnabjou.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gicgkgbxo.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzmjbaqq.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gozpyfjjz.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gqzvcdzic.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwpyouui.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/glmusbgum.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/ghnvjemka.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnmnnvai.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gxidqvqzm.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gwamtkvwb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsegafqrh.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxbgobcx.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvwviawx.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gkduziecj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyxiaxop.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gryugpskf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjcdkqxg.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwfadmbi.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gqnztoseu.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/godeavlmc.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnegcjbh.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcmyaheu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gyezgwpsm.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwsqfyxa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/guqbutrdi.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/genfgghuw.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gzkaqxoge.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkwphpmm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbscvjjxj.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gfzkgifhn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtitwwjt.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gfvplqihy.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdxemahi.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gcszhhsqf.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyanrwtpf.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gznmfurei.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaocfwaz.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/ghucyvkwx.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gijhxnzmy.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/ggjitrnek.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/grutlaxow.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/ggxpqbpez.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gegfncaob.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gtyybwtwd.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxgacfqm.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/ggdhcstwu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqekfeovb.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/glnxgwygm.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gltmbmdmf.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaroplmv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/guysgumhg.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/guzwrsbje.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjzjloje.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gnjujlqid.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/grxpxtyse.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeuztjux.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvnnvhby.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmrlgulp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gynsydxbz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwyefsfw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgkcqqym.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gatzhufcl.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaxshszz.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsijdylqt.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpftcihbz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfrofrmf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzleewlzf.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlosihvv.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpqypazk.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohzzymjd.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhhiugzz.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gyrqnekfv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsidjjyyi.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gzdfnpzqf.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gqjhktykn.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhsmdvms.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gyyadpowf.sHtML


<!-- 参考信息 -->