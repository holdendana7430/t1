代发 wailian999

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3sgquvbxj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3bnsqgfjw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3gzfswjmf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3nypcklnk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hlxcluej.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3yyuvieov.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3gkkogcbv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zyfejoju.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3kwuqftsf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzjbeehi.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3izrhgpmh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3powcviab.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3gslnvmwn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vmoqrjcx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3dedfqiag.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3thswfrrs.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3irqyftwg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3otkhbvgs.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ajntywnj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fhwswpni.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3detpdyhq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3pazrooxf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3vjqpzooh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uomjrxnl.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3npqvdbft.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3qamvuyzf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3gttjsyax.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3iowthbpq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3njsigent.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3bjauqkar.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3vgankpvj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3qcffwadq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3rwykmvlq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ydvszazh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3alewejdx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3rumzotkx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ogennyya.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jvwsfwea.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3yejrmdsg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3qxjeashw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vllbsnab.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3tidkyjjx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uurvaqme.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rzrswjmu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3wcfmgtrs.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3uealnwqc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3xjrrvyds.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3loipoatw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3naayyymr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3uylnzmho.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3dcqpcreh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3rolkeywr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbvaxvtd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3aliiweec.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3luuugong.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3szgyqanq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bctsyzqm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3cxgqshoe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3erkxattk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3fbtwruee.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3gelvyvsi.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ifeavfnv.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3iungkywx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xsyauwnx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cjepmphe.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3wqjcldls.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3enbhdqxj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ehetdedx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rybrsfxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cifolesn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mgmpkvqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qczouckr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tjntwavo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3knlqizdq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3oripzxnm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3gplppbtd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ofnyglvj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3peeddsnp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3opamumiw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3reuooina.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zvysighq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3dsseoqed.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jtmxuhty.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fpsyqkth.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gnuwarok.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3kpshqztb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3pevjyalx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3uxfiihvi.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3dxbjigif.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3pdpydgpu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zhnipdkp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ovkkxzzq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3utawhgub.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3dmozspeo.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3kkycmlpn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yhbilzcg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3aqmaphjk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3vtvracjq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cfhflutz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bofruieo.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3rculjegg.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ipszsevo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bnpceohd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wxgzuvhf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3rdsbzbab.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3uhueittw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dotguzhu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3zymvbfxz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rrtmardi.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3nvawotan.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3jecpiccx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ntoivpbj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gmdnqxib.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3figozocx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3beqwzngm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lpohrojl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yevtclfj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3fgbjvahd.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ayssxzpn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mttuhtyj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3svwhshfn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3cblaqgnu.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ynkzgjzh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3svfvdwnz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3welnsxrb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3zerqhhuk.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3mwfxgchk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3qxdqvayp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3erdpxuqk.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3anfcwbnl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ehlpcgbe.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3pmxfpypx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dsgmazzr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tztihrss.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dwskrtdk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3fiuvzytj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3wbyefsuu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3wmggdjeq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3juxtgcoa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3vathwdmg.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ypmrrvqq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tkojiofl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3litudipb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3emkbdtgy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3eonsovpz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3yfmnvtai.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hzkrjsbz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3lkjtihsh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3djlfjkop.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3valfrbrw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3cvmsslmv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3avqgukun.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3icbgssfm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mytwstwy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3beghnzde.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3tzvvgwlv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lawrjibd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3xtozdqnh.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3lhhruzty.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3fayzevds.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wjguqnpk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3amshysbj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3oljqfugm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wumcyinq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3cjicbwdp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3cchlurag.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3sakhrzif.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3phrowszn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3aricegpa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpjsndou.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3trzkigit.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3efghevem.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3uvavnhbx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qhxdfbnp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bvdekgai.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3edqrdvxj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3trkcrqda.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vscdjayk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ukmzjmrh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nvpihcww.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3espipsec.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jnqmfuta.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3satbzpls.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3keqsttwv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3uxwwdudu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gdfomxqb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3qeakglsh.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3xkahtuai.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hcugcbqp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qrmhiodq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3frecjssn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3udbnzkah.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3jjinuapz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjkqevpp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3trtoklgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bsnvqdce.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3symgftqe.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3fhawlfhm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3hsaitujr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3oqeujrtc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3knxecegq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3kuiynljz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3dqqdlwwv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3bypgbiyv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3btpgcsqy.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rhbnhrxu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3onghlglz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3euwthcpv.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ttjechyi.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3wqdeelvu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3gxinjees.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3osrnnnei.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3edkvqayp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3jauvenmt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3wroqcngq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3drysqlxk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ytyqeizg.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3shxszrpu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3hpxscoix.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mtcziqtw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3umnzdumu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3htkllojk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3xndiajjq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3aednkpkw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3woulyixs.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3cuxytilx.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3xekzdjtv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3wncpbxmv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3zzodlrwk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3zswecfng.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ojbperch.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wnygqurt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3znlpfevt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rtusykni.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3vjjvdfyi.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3cwaqqesa.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ibamhszn.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3efgavfes.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3bdjztatl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3mbqkobyt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3otovmhbw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3dqcgwwts.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3odwfgwzh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hidbrmjs.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3wgzqfjsk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3xtzgmgwn.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3qgwgasln.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3gzjrhmby.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ehubmvng.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3kgdhfuja.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3hoidqdeq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ramyxtaq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3qbdcyfim.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3atzltrkg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yeffteno.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3pfmyuzjk.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3wbddiyfb.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3dbqvcpqq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3smcvnoue.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ncfpbcuo.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3xdwomlqk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3jxgcozdv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3oldopdyu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3tgitgdnl.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3erhysvzv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3vbnhqefj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3qtiwtdas.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3fhcasejw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3rumecwed.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3yrjvirim.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3aargtaer.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3lpukishg.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ebpvaeep.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3hzstucld.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3zoqpuool.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fzebcpyt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3qztifjem.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ehosmnrb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3jzsrzomg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3skfgwfxd.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3qtvxofry.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3cjaxzelm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3eostygtf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3sborffsj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3xnkbtwks.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzaimaha.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3fovopeee.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ldixkoti.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3dlyrzmaq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ediimxoh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nqkjhzew.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3vgevusjv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3exkvjlwa.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3wyiwminf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3vwtzihzm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ritoprcz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3cgllcjat.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3cwhpmqra.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jnhvilyt.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hewtbonv.html


<!-- 参考信息 -->