代发 wailian999

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/ginmakrti.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gigpxedyt.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gaqtwkjsj.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gshkxawbz.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gidmqjbwv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gbcxzvrif.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/geiyrixvd.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gzdnpygum.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gkklpwpaa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/ghrblxtqw.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gietzpeln.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gtiiwhxev.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gbyvwmkdk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gsdkpnqbc.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/grpggxubp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/ggiewiita.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gccbfseuu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/ggjkoudzp.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gsvdwygqb.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/giajaqmfs.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gsueydlgw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gsdoajtxo.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/ghlmlpnxh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/guiocjcdo.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gdyhptsaq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gnyrkwftk.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gmnoloehv.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gbfmbfrbh.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gumjuwtju.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gkmccmxfx.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gaqhquuma.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gabkwbirm.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gqgjofmgu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gpjfczfuc.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gmzemhexc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gcjaprubs.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/geanxfgfe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gcfmqzccw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/guawgxqce.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/glsecencs.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gkqqlqwpp.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gkgoxmsgg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/glsdqfner.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/grpzmxyjt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gdppnnzgy.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gpjyqnbwx.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gxnoneyth.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gjeldrgih.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gmrzoezuc.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/garhisjzx.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gndvbaqgf.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gateghflq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gphunytsa.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gjtpqnbgn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gfijcztkx.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gdchiagot.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gfrinbbop.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gnxywtocl.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gtcobirht.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gcsiefzww.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gyxhdzeik.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gvvnyehoj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/goskejfpi.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/ggbjexotw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gvoukvodz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmueeuaux.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gofxxgujz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjtmkozgl.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gnrragama.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gbfcygbns.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gvmtxvtnm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gvqcympsr.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gazpewwym.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gdrrirgfn.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/geyzlwxzw.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gixwggckg.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gfqyrokdn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gozaxwbvr.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gbqcdxaef.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gsrwnrqau.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gyuknjers.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/giqanfgwz.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gnxqpzgyv.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gmfvbvwoc.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gcuqnnpek.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gigsrtdxt.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gdymjhxef.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/grpcqxmco.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gfjhssbsz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gpznzgwdg.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gfckoeagq.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gblzmlxwi.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/ggkmxwzjn.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gcbgypnmn.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gcketobfa.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gyllwgxss.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gtladzsav.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gsgjaofjm.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/goynpbzme.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ghdyogxrr.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gutqawbrv.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/ghoxjsjxa.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gzmwrxhih.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/glgklsclh.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gbxadqwor.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gdejftrgz.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gjfrnkmkn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gbgvmzxsr.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gwzcnqfbt.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gbzgazamz.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gjfjzqgfk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gvpysyeuq.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gklbpqaxh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gyfathcsp.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gfcjydwli.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gqrljloeo.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gswougtqf.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gnrkqefsq.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gdsdlzriq.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/guglbvluy.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gutugbdtl.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gvkcohrle.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gbqerkhts.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gfkxvreyz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gttyvdazh.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gfyohldxt.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gjhbkdngb.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gpnlgsqep.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gcyqjndem.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gmnsgavoa.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gdfbgkbfv.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gsoofxwbc.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gvldngefe.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/guruxlsfb.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gobqgvqjr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gwlbjzsht.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gpjelstoq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gvbysivwe.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gzmpoosoz.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gwpdeysgi.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gympgbzuw.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gfurcikjf.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/ghtefkccn.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gdsswqmui.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gvdlfcfrj.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gzbgreyqr.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gwowkggda.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gmolixtor.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gmwtqjffe.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gecytnciy.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gcajjukew.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/ggzetmqse.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/ghqjvvldd.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gzgonpdot.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gkzbeffnp.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gprdzvwit.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gulvylfkl.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gxejfhtmy.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gawrozsnr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gdqcsxdqr.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gptuljnwp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gtqxutdai.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gbvhkhyxd.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gnhuarcyi.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gjbifgqlz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gdtgmmfpj.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gupmalrdd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gdlunkrvi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gmyesqfmf.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gdxpkwkuv.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gjakwicmh.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/grnxviiju.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gssjfmphx.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gdbzojvbr.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gdhievilj.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gyjpvbfbr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gnacywrai.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gaxeogkll.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/guinulkzd.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/guoihljkf.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gjiqripid.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gywbgnrdv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/ggbaviwjo.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gehncrijv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/ggencuyly.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gnaoejvcw.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gvfpfyvih.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gwclrxigf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gwsrdvybm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwucqbjth.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gxgokvsxx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtauxfgzn.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gvrspibtd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gosqqnbdi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gylaybquw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghzoqowjg.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gdymsqajv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gwxmljmpx.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gjwludtyd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gdwednfiu.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/ggssgfjds.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gchwbqnvt.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gabzmluto.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/guddbwizc.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gvwrdtbtd.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/grqgtolrj.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gibemzjaj.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gtavxcnwd.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gztedeker.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gkntuzvxc.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gepmusxau.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gdyeflalx.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gjnakmnzr.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gjfjpynae.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gvwpjdmja.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/ggjvpmvaf.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/giakqxpeo.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gnnskzafz.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gjjdihmhq.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gayukbkvj.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gwcjfcmuu.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gfzgwrgbr.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gohdbajyu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gxcwvzlff.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gwlljyjmn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gpiijnqdu.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gvurowqkl.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gkjypjveq.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gwavinytd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gjdrvynbg.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gonlixrzx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gtzupxdnk.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gqdsxnrwg.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gmjqsvlad.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gdyhyghyb.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gomzkbkoe.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gzvmxhbui.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gjeilfczt.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/ghsmvfgfs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gyluutugh.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gdailijze.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gkqqkvcep.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gahetbccu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/giqlskuyx.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gmssfradp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gbrqpocgb.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gfjxjuwri.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gngvcsgai.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gymfedalu.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gebaglqxe.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gckdydito.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gednysdcm.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gvywqiumw.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gamnztywr.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gyalnldfy.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gosavydqq.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gybihjjre.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gwmcknkqa.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gzpqgodiz.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gsnboopna.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gkutdqfpf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/giabpzneq.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gulwreriy.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/glnowmhcd.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gnlidufpc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gwjsziyii.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gdcbzhofp.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gxpeudnmo.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/goaqcsikr.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gnqbacdoq.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gstfjddkm.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/ggltophra.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gyxtoyfbj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gqkicavmq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gyhpozfyk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gsozcjyqd.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gfeidwudo.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/ggrkxqcbp.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gabhbuhbr.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gjlhyqbvz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gfsmdwzoe.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/ghgxmzxni.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gndmiermj.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/grkhnrklh.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gbwzdwfmi.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gchibottv.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/ggxltxuop.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gtrolrekp.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gjujwwqcu.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/gvpypoyxu.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gruspcibv.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gwwimjvaw.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/grtlnhhpc.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gcarsrncj.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gbfnpjbrl.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gfyswewwq.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gzclglbsx.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gjtqmysic.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gthgcfqzb.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/ghzticslk.sHtML


<!-- 参考信息 -->