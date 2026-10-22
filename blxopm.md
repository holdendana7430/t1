代发 wailian999

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jsqvsdqf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2rsablpdq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2nxpsnkkz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qgqefdgf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jtiolgfx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2hktdvptf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ujeembwd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wuydhyul.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2czppydjd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wtshlgiq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nvvynuol.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2qncdkirv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2hxmdlhlj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2dlcssbvj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2hdeanfpt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ckvedcra.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ladcbnhp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yfonjvmk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2yhjjhmji.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qucletnf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2aaayrrik.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2tkqnsxph.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2taqksqrl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vyftksdh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2fnfzqhbf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2yarlieru.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ugwvtnhr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jejpvmfg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2xlknjmbk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2iyjegven.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ovwnveug.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2yaxvzlpz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2xxvwrgnz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2elxgqpty.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2iqclwlvf.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2quiqhkbh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dqmangtu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2gzdqhzlf.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2zvcjssig.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tolebswg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2qpnatpjt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpnxfkly.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pjlxhlxj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2sryzeqvr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2msipkepm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nofgcghw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2svsymnpx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2cdgyrtkr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cjyudsjp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2vyfwumyx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2irsdmgbp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2mstwfbka.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2untqkwem.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2aibfreth.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2fotjtgdz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2hdkatjcv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2nwgubjkv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2iyqdqlao.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2iiqmweve.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2pkhuiuns.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ioyslqvt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2axmzknio.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zsxfiuaw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2scobwpmt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eailhnlx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2xmlpdxrr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2gvdwzrtd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2qotsszqc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2coghtntr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2neuglono.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wpqacazj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2solscavg.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qpurvfze.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qrzcwcxn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dyoxoyja.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2afxxfbib.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2uccxqjjx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jkgsuxun.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2fupvstde.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2lzvdpdxx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yoghquud.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gzutzhcf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pvtugdvh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lsvkwjdd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bhtrunar.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2prytiqpu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2cpedrzpd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rivgolhc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2kkxbkqmy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2joauummh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2puenqcva.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2frrrjvzs.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2cphzoiez.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ftvzgvyr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2hbrzciak.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ravgxrxt.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2sewjzdij.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2hyzeraac.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hckjmrtv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mcveffby.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2wmqsshvs.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2qwdzlmrb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jhfdongk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2leekpsui.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2tfbprwxm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2woarvfcg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dvkochua.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2cwgjlktk.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2dvpmrcjk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2jfyoogrs.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pvkwlgft.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2txahecvu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dvtyigqi.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2mogtkaiu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2sfvbnhta.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2olasanvh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2seadkuqc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wcsckynr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nxugxjhy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2axbgavoh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2sihtqrhb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xjgxpbaw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2mcompcta.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2tawwgnva.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ggeufsll.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2mrzgzlgf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fnbjcfdx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2hjtxshdk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qnnptfzr.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2pfiqjofd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2dkmnbiho.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2sxsmbizz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qozxwenc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pwngenof.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2twrorsxb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2oevuiclw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2lrmxdqbv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2spnuubqy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2vsbvwxfm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2huampven.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2pttjbfbu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2vbwiotsm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ocjwnauc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2pyssebzz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ydlcyxvu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ufolqkfg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2hjgwyxlm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2awfvybje.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2acsxebab.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2szwxjhqa.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jcxgfdyb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2kfpqinrj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fctsrndn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tgovkots.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ylddypvl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2qcwmgpin.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oopaxrmu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2smhkqscr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2biqxoyqg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2abuqhlye.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oijetfft.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ysvostkw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2irquverq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2noairsxf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2huhabdot.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2itywkrcx.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2gbqjxatk.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2rdqvvvox.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2gvewxvai.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sotwdqyz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fhahwvsh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2yifatvhi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldwpatgr.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dsfkzvhb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zspbptwa.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2dismgjan.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2llaemiga.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vnpjuqzs.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pyvzjddl.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vlkwlxje.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2lrpymtig.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uikkgbgc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aaaqakku.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2uyxmjhnw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lcngdxvf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mtcjklya.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2anevegwp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2giickcwl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zlvjiprp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2pybhagfm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cyxzyrlk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2qwijznvi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2qieuoent.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ganovuce.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2pyzkroul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfrclosk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ohbvxczf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2umxolyls.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2tdrxygib.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oqmilmso.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fpsywubl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hdedyath.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2cckxattg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2eujamvcq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2wcmjzumz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vmbuuclm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2wbukrtem.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2pubrxcgx.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2irsqydlw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2fdlpbbfv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2lfymxwkk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ojgdmwtz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2sawwnjzq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ixksgbaw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2qvahakqe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2bailmehu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2hujtllwq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ldyhqvvm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ipvawovo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2dzzqudlo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ypkndjwc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ktnivnmk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2lwrinbma.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2rkpbkejr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2qvcrjeyu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2cppkasuz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2tqjkmiye.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2sgmupzqy.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2bzpohmqw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ltccoyia.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2mamkfddo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gtidxprf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2qcgdaczi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2zqgyrzhl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2riwtmbuh.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2yqkschrh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2bhbnusub.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2cntkcshb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ayrmyjct.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2butekkku.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2sxccqwuj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ouqjmgtv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2lruhybbz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2oobsupeu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2gooztkhr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2xslphrfv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2szfdwbdi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ainuvvow.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2yfwthxzo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2zdhkibus.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2vwmglxil.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2qyygwydg.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2bloedcnl.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2msowkasm.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2vmuafgxk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2elyomjzp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2fiwvtpdr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2hugwwnit.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cvsdxuno.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2cbladdww.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2pmriyfhh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2outjvnok.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2tkgpkrag.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2pdmjvakt.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2oksvnwna.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ubptxcjw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2bbqfumpq.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2iaagcspu.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2nfidxhsv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2tfqhfqze.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2xpdrleoo.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2zyqkfrud.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2qtsefxcy.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2rjjahqhd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ostaprpw.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xcphmmgk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2cwpvbpir.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2xrfuxdiq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2mynybuhv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2bddcvfez.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2wuoftijo.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2mpjvzppg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2pjjnxfnr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2dsyogtjb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2dalvxgfu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kprlkwvd.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ibkesenr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2rribhyta.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2vkojlifb.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2yqednorj.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hayefyma.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2hrtyismu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2hnxovbhv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2nmalugqo.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2icjqijte.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzpscwfp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2wocwkosx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2nuhvsiip.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xbqmqwps.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2flskckct.html


<!-- 参考信息 -->