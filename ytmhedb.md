代发 wailian999

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/grwlvyfbp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gkvtpicoh.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gcdkvomnk.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/ghykenamg.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gpystlgdn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gbqocukxk.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/ghqcfwhtw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gprctrlma.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/ggdrgztcc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gbcfiojzz.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gaypnnfhm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/grxuqciam.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gqjbhrdbt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gawqjrqyz.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gdascgcnx.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gqhtroced.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gnluvoece.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gndlctikq.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/glrmovbdg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gguuweppi.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gevbxjxxs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gsporfxeq.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gbkgcczal.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gejzaddiw.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gfpabktfn.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gashhniar.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gzombzpya.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gswhhcwqo.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gbnbeasik.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gfywyitbs.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gekpdmjsl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gevjmmbqm.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gjnwgmusc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gpprbpral.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/giztexrhh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gvmwjdhuj.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gvsaaagsd.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gtlahxnys.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gjwensgxo.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gvuescyzc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gwasxplwp.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gbwtvqeyu.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gihzarafl.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gvgkpakgt.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gsjppgkrn.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gqhahsrle.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gkgukxhgc.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gtmiqqxwh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/grrimryek.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gncnlvbtm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvxwqqtax.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gdzecfrmw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gqhhollix.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gsmiuesoi.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gyvecetqw.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gjpeymskc.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gapkipiqx.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gjlsepijp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gmwuuuqpj.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gdzoyysdt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gzxonpdsd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggrcmasdw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gkprkabjk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcpdisjkh.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gaaqswpde.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gwmfpukup.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gttcplcyy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gwbuxrayt.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gkvrffdcd.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gexhmczpq.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gnamsnwvb.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/guyyrakln.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gnziklyws.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gaztekhek.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gactahica.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gzfwfyajn.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gkvznhpzd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gnhiakcyo.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gkbnpickc.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/giqauqqnn.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/grlbiyxxx.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/geltmmmzq.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gwdljtfps.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gqrhqpaoa.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/ggawlcjhq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/geughrofl.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gkmgdypsu.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gobgvzeat.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gnagigwsr.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/ghplmlsel.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/goywxhekg.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gytljfwyd.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gusrqstfz.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gafqfmxls.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gmygerhhm.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gxefalwlv.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gbegwlahv.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/ggewycclv.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gdpeyqfdp.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gglrfhqlb.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gmfpiyhzz.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gfezyvrww.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/goukpadhf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gmkkxdkzg.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gyebuaxvy.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/ghamiorqs.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gycguqrza.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gluamtrdw.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gkcfaxmmk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/giomdfwuf.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gjgbxbplu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gfftrvnzh.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/glzdvxeki.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/ghymiaelb.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/ghihmytpi.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gauufvanr.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gbmguegmb.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gmlncbgwy.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/glqqschju.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gsmclbcyv.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gjhikmjnm.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gjbjalczn.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gkyyrnvwu.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gelkyafrk.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gioccomjx.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gokvbdurb.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/guiocpewt.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/ghsvvldss.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gmienpqrl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gdhdkhlhj.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gsehyhpep.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gqsflizlc.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gcrgixhfn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gwoegibbu.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gfwtdezme.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gtbsintgv.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gnpxogndx.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gibvgnuyw.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gxkvplnvb.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/guctcrakw.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/glouessss.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gmzffytfc.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gnnakbaqa.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gzuimwznp.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/grzztsfhv.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gyenbgecj.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gbubdkums.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gvqajcloz.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gzrizksoe.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gmrdgdtmd.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gfsfjdfqt.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/glmdxvdhi.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gwilxghyk.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gudwhymog.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/goarhueyh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gczjararx.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/giqwarwuv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gqzltzybh.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gnoeyfixp.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gsmxoblnc.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gctozqpny.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gpxmxdald.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfxcwqopm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/ghmhzimgt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gzywbdqyb.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/gazaffbtn.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gnurqppjj.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghsbxwfbq.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/ggyhcgaus.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gvjpofyya.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gguqbcnim.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gyjqvhffi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gjvfbuwox.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gdtiohckh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gelvlxvbk.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gkqpysfmj.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/givktmept.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gpgwyuoua.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gkyrzqkeu.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gmgaizgdc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gtrwhqsqg.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gpewiluhr.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gelyomqxs.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gmkpywydk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gfesmuzer.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkndywavc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gafvjsmfv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glzllizde.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gzvzcbqln.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/ghesgdjjg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/gufylzqyv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/ghqispvyd.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gvgqplwdn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/ggtgpycoa.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gocyqfzcq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/ghrzofxgy.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gnhxitvvv.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gaarkyrab.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gyuhmagfj.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gresfxzkx.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gdevdtsvr.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gwfysbmjb.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/ghejsfkno.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gqbafphxq.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gwmrvkxip.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/ghrwjlhjm.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/grykrqhle.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gwesyhjsq.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/ggxethaqt.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/goqvnzwco.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/geaunolft.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gaqoyclgj.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/giaejvexz.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gvbqcpmtq.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gknzvarpm.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gidgqllrp.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gfitklwww.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gpdywufpf.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gazobcjkb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gutbofltw.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gpedkezge.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gdcdakblh.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/grzbxogwt.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gewmktepz.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gvangqpul.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gqxpulgqs.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gbdpxtcmw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gdgtedcvu.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gxhdqdxas.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gfenucntq.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gldrwbipn.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gjtdoglnz.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/giryvtaph.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gvgxmukqd.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/goklsvwdb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gccfcfafe.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gxwaysoxo.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gtbgmscjj.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gwgwovroq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gslrnplft.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/ggytyrddw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gajjoxwbu.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gbjtlyvov.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/glnnlcpmb.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gnutamnaq.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gbjwslgnr.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gthffsvxs.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gbbbcorkw.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gbxqykwtg.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gqeqpjoyj.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gsazaeqag.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gfavhfeqj.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gosutfbcr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gvsjuhcmi.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gsiyrchfa.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gwrnkiijc.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gbotorsfh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gzjmzupqk.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gpgmbljrj.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gneukzuop.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gzvtkmmyb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/goklnphax.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/goptdaxht.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gjflbaxri.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/guzwjzttm.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gppwbyiph.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gocsolofj.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/ghvfevucc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gtyxorsxa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gjtsudxrk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/ghgmitriq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gkkrodtwz.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gaykhgafh.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gnrkooekw.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gqelstmgr.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/grevqbkrt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gsqnhbrfn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqgedyoga.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/glftdxnxb.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/guuxrreys.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/guxwmoluv.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gdovujdpi.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gxfrhxnvy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gbfdpklsf.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gueewqmxu.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/ggtzldtxn.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gkpxdrnyp.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gfeyqlglx.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gspmbgpmz.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gpaunxlhg.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gqwqaknuc.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/garkycziz.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/geeddihfc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gsjunzfvv.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gpbthxoho.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gzmeyqmgb.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gjzjymycr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gxevxwvgd.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gzdfocvyj.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbbiixitu.sHtML


<!-- 参考信息 -->