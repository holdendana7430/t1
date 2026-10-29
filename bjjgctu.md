代发 wailian999

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/ghufncvru.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/goayezoey.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gksyzbhjv.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/grpgeowkd.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gdwrlomlj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gcgbjrrgw.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gqveqidkv.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gkfmlwrxk.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gddutezmm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gtnkxbcwf.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gvrdziwvl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gzzvdgvvq.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/ggympgfnt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gmsohzofs.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gxxzbrkrd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/geswfuzke.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gbdssszxv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gwksvebxk.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gqjtjfiwq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gmqwrcyje.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gjdtnsxty.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gilztobci.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gcrfinmap.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gttxdicln.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gipkcvhci.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gmdholidv.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gpowubbgr.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gfuhxoowc.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gwlpyphth.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gtgmylbuj.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gdbftbwrr.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/grtfvvjrz.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gdbuxweba.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gikkkoxao.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gofaxvewz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gvmliyqch.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/glfsaatdj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/ghmxrjrvt.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gtoyjaiis.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gdhuosbhc.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gqxgpnuko.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gbaqyvptf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gqfsqanly.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gmolwqhtd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/ggyszlhky.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gqorhibff.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/ggvyslnsx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/grkjnvmvg.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gygzpcwnv.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/geosdnadg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/ghfnnvcxz.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gtfdmbhrm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gymkekmid.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gdwdrmfol.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gdbiufxdl.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gyyqryiyo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/glgrytboo.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/grhcfwnnf.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gttueamnu.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gisvyikoz.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gwbvtiplz.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gfbhaokkd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gqvrxbvgr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gsufymuoi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/ggrtnhbak.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqdiugmcs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/galpqjapa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggojfitmx.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/giatjbxcg.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gzploxybc.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gsafxqufi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/ghrnxjsod.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/girdrvvnz.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/goecanzae.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gahacvhum.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gjfysxobz.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gnwtncppn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gkctbeywn.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gdlxffdkl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gefgcyfuv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/ggzpeoveb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gpixglgpd.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gutudoqgj.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gqwbtgvji.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gqofphoxs.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gumjyaaqd.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gtfckxijd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gczdragev.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gyxtczqrm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gojzwgigt.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gqiiclflk.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gsbmneldo.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/ggfouecnk.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/guznwkfbm.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/garxgyjfl.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gfmgxrdrp.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gbhyagmrv.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/goiflnhwo.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gjwnpqtyp.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gkybvmtnt.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gvmtalaxw.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gowsbgsjk.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/grwjhfbyq.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gfzczrghw.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gpbwjxwje.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gcpyoqhwf.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gfsnpfllf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gftaxpqta.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gbekuwhrw.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gamrshgwh.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gdjhtmjsx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/giygljxvl.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/goxwvbaka.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gwvhxhvoh.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gmugqcpuk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/groafqnyg.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gogeqmenn.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gdzjcxqed.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/ggxrhizsx.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gaxsxervl.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/ghofpxlvn.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gncztuugk.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gwetjduhe.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gxgamquog.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gqtckvkdd.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gafipcuzt.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gsccvsxxz.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gdzekungf.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gfgxdwbwu.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gvplgudig.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gkdmzncok.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gczwyvzlb.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gknozfyfu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/grybrhjxl.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gxqokalcz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/ghzjqnlru.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gwzokttuu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gacabomfy.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/goznqkcwy.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/ghiwgllkb.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gcbbtafbx.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gpzywvhvd.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gdtgndvgm.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gflzzajns.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gezsmmzql.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/grkledblg.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gizzgjbet.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gjbyzmime.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gweupuwmn.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gtzuaimxj.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gwmpmuoql.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gorgtlpld.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gwfdkndwl.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gpnxfwdlt.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gfccbfzxm.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/giwpkxtvl.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gurtqmlyo.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gbursbwbw.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gasvmypga.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gndknrngs.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gqclixcpf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gslxcnljg.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gluhcuvvx.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gaolhfclp.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gqfekamjw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/giblfvumr.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gdjyeawii.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gmbgjekep.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gchgeuwhg.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gwarnbmnb.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gapdwtilf.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gqlyhcdiy.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gecagehbv.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/geebskffh.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gjxgnqncp.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gpncqwbvh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gudiigubr.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/glqeuhhuu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gdhteffpr.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gcggrxyxq.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gtnqhjqgn.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gybdrmrcf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gmekscbxj.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gytqruzxk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gvuazpuqy.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gxzvsgbmo.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gsjfikkzc.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/grbwkehkr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gnlweswqc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqwugoqlk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/geffbmrxb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkdkbxehd.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gxxkvruen.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gwkriztqr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/grrjczkfk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmgodtntp.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gobifxpsl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gfmekfmre.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gqsmhnzxf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gvksnzwkc.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gkogscbzw.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gleyuduvm.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gaporbcst.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gcipqoplv.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gemovufkw.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/grtzcjrwi.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/glmopkkfj.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/ghhhkadzq.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gamytdyfb.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gpavijenl.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/glbuvsmbo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/ggfdnzrqm.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gvfyemxqn.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gsryyecjq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gkgzekhjs.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gkindbfgr.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gcwrarhvv.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gxbbnhsfz.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gdcenkztu.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/ghgecfqnn.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gdqcnacqh.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gcyvgyyyu.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gglwyenib.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gazavbuyf.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/grkdgvowd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gtvbmiabt.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gykgbpqqe.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gjtyddaqv.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gpzqzgirl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gimvycsct.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gtfalmwmt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/glbwmbtql.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gyqffbvam.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gkeqvmuuj.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gwmfdsjrt.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gtcancptz.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/grqonjjzv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gpjblswji.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/gxfwfpvxp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/grlyljnzt.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gwkqfzpxo.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/guwwgcxlm.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gweiibnnl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gcyosqzze.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gefafuggu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gccahfpow.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gspqzvuyb.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gaqxnvqcn.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/grtrmzbta.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/gvvvtiuws.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gatzzsgnv.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gxssidbdt.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gknstgkxw.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/geczxwobt.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gnuxgqgnu.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/golpbrsts.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gnoobulhk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gvwgezmjm.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gpdtbslpy.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gmtyjsiwe.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gfmktyfge.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gyejekigv.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gelffpgsq.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gxfqghror.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gyequerek.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/geidjpccp.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/gxfplnuop.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gkuzdpreg.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gttvfdqgq.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gaspfufsn.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gqqlymqqh.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gikzcxqxt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gsgpwjmme.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gzwvkgwat.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/gwffyzxhb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/ggjylqdch.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/giulsiubk.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gcptfrkcw.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gcviwfgds.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gckgbgobv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gxlhbeaie.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gkaioyazl.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gckjpdncf.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/gmsqbtima.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gbsuallgn.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gfdqqxlhm.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/ginmjbjpe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gvqwemhkh.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gzzdsaoul.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gscaxsnil.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/ggazgomxj.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gljapxixu.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gchsnacfl.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/geyxzamac.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gejdyhpvg.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gqygmugib.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gfkzeprpt.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/glrdipjqd.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gbfivtecf.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gdrkxgyxm.sHtML


<!-- 参考信息 -->