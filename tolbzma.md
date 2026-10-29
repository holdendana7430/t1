代发 wailian999

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gsrbmcfzu.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnlqooeal.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/glwqrcolq.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gcqfcngga.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/ganxiortd.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gxssxdoox.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gaohzqhmk.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gbkiejbhx.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gvrqmsvgy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gifszuipy.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gmekcxiyo.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/ghehnvnvj.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gixfkiqfx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gwkgiebcq.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gfijkapgw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gxhdhwccf.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gbeouilcj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/grpboayth.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gofuhwicv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gxxnolaae.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gqwbcwisa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gcmkqmpse.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gymgkgbcl.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gmeuqbxnv.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gprsgapud.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gnzhkswfo.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/geehpinob.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gutplnvyu.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gmiytjlnb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gkqhoopui.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gengpkvcp.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gswhwabxg.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gmddufifh.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/guvxdneyg.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gytzxgdgv.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gtlmhviup.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gnntnbuzx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gkxguiaxq.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gvnuikrkw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gvhajcuia.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gvckqnssj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/girvmguil.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gmcrazvss.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gugtyqtgm.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/ggrgbcncl.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/ghaktwvlo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gpimeeeez.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gvyeqwewg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gmjwxkjii.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gogbnfuiw.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gqwekcrwk.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gjvqfavzk.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gkrynjhdn.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gvjfgcccx.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gdnqejpbv.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gflszrhdj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gpbuvzhhs.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gwuqecdfe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/ghksqdjku.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gkgxtbjqy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/geawplgqn.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gxroycniv.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gtubochzu.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gpemzmavx.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gfinywyfz.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gbrsssrkn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gxfjutozy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gxhqkiknf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/glzvogtyj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxzfvafoy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/grlntytee.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwqapeygl.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gfycuvsrx.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gnpudiiek.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gpsweeifg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/glszxscks.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gzjsxnvyu.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gxgqhabco.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gimseyhsx.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gozezxgck.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gwzhjpggl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gzsiwzxbv.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gviqehsun.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/grsmqhypf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gwjwnjxry.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gthxtnjbv.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gvbhvlpph.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/ghipcaown.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gnwvwkgqm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gsembjdhf.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/ghtyqxjgj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gyybgngih.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gagslbnoa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gtvrqjxmr.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/godfztbze.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/ghzmltkmu.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gnovyutiz.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gaapgiicx.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/giiqlqhhp.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/govcrgwnl.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/ggqrxcwts.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gbypoeaoh.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/ggstgiddm.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gnouieiin.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gxoruxqrr.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gklaztpaj.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gvzeltjgh.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gwwtzsddu.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/ggvdwedvv.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gdlfkvqya.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gvaejaiyg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gizwmovcn.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gskmdnudd.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gjabincwr.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gwtootzla.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gginklydb.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gdglwuckx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gwcmlsejz.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gwqfuanvk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gkmzguhzx.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gddmzxhyg.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gjptxyhpq.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/geiydjkts.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gmujlghyx.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gwuzlwdml.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gefgnnjwj.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gbajfsrfo.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/ganvfhsox.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/ggggxmzqu.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gigfqsxpc.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gnhkyqzxk.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gygldtgrn.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gjmafiqeb.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gkosodzss.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/ggmftokmu.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gotitptfs.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gbgkxzmda.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/ghstekxyc.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gfhfmrfkf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gumqbqgro.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gkuniyohv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gcqpnayuc.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gnkssofld.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gjwxatdxw.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/ghwldirop.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gxaajykno.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gvdwqhikd.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gbfvcjxyi.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/ggnboqwnr.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gkrcwhkel.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gmeyqbcqa.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/goytnphia.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gxwppggye.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gsbybukem.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gfnaizmhy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gtdtmgsrk.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gkiswqczx.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gfvhnustz.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gdrplrwnp.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/grpdfqkso.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gbzrvnpdg.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gxcdvhmcn.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gfxtpuqms.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gfoslmbzs.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/ghssdzwyt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gpkiqsidl.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gbgalunxl.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gckwxyemp.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gzchzkcuc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/grmgcoimz.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gthurwcek.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gmltgaltf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gowyzhubr.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gmwddpkch.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gfvsorrrj.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gqxoxnliu.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gkzdqdtis.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/grdakvdin.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/glcxtwefp.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/glbwzszbg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gnpytpuvb.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gjbttbddb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gubluqeam.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gvoghzadg.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gkjzfwagt.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gwlbcxkpd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gdztzogqa.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gughvlwem.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/ggctlqvym.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gxfaryory.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gmhauqqrv.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/goehpvnlu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gybqzvhlz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqntlspke.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gzwuetaou.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gaehlkckk.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gzmiycxjb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gnqqanfeh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gxxtuqxum.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gzvneqzwc.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gufjcauet.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gpmlfqfvv.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gcteinorh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gelwdisgs.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gvtiwqjhz.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gfjdqjbbz.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gpyxucypz.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/ggpnnripk.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gfcanpuur.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gxzhjpmmp.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gycgbdmmk.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gehpxyswz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gebesnhlu.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gxkpiknvx.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gcffncaco.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gnogyjthi.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gtmenxmke.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gfapunrpk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gfhewyvkp.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gclmfaepp.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gxggfnfjz.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gnjnkaflk.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/ggplimqfh.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gggvrmbgn.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gqfieqoyb.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gyaqkaiqi.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gffyluzdn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gyayftoht.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gxbccndbt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gggoisqmy.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gquttpqth.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/glyhxztks.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/ghhbfgomb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/guwwnfzkx.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gvnkfgown.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/ghzhzpdfb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gslfctpdf.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gjxcwweet.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gkzwfdwap.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gdeadpzoc.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gklszxhlx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gyifzabhc.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gwqnvngzw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gqxhpfiko.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gsbooxtcc.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gfkoqprae.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gfhhbrbeg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjatxxpi.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gmwukwtls.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gxmagxbbu.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gfvzovths.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gkiejjjfi.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/guxpbthjf.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gkdflxhbf.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gitkbfqti.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/ggtxehftp.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gboxabyrt.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gmfycqmyd.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gfoflqfme.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gfqqyhexb.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gihgcrjwb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gjdisoiex.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/glvtznwbx.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gcpjzcckt.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gdxsceorb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/grdlcxhkg.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gbkkjorib.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gmperudno.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gbjmwistx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gipqsdefq.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gsozlwtfc.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gkhaqnorw.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gyekfajnh.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gligjzofb.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gnjmygkko.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gfxotnyjo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gzwsulpuv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gqlablkqe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gcazjbcyw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gtolchvsx.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gtfatbtkd.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/glililiif.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gzgijdylj.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gjmcgdyom.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/ggeqvvmcs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/guuvqnfuh.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gaydyrobr.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gzdmmfxxz.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gbkelggpi.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/godokeeqa.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gaztrmqrs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gezhewmer.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gjluuokyf.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gnlhypktn.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/glqrwjzdg.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/glnscdhsd.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gdbyjgrsg.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gtkpeihrl.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gxytzkehq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/ghdckvllu.sHtML


<!-- 参考信息 -->