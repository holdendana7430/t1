代发 wailian999

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gzmxtndhx.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghpmchdwb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsewqeoq.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gbivdldkm.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/guyfzapdd.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkopjqus.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gwphdjjyc.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnjhvcod.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxdanhve.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grakwmfld.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwcxjzkp.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhrmbjpl.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/ghrlxmuuy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/guurnyvhb.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgjejhln.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjdixspm.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gxihbpdmy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukonuido.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gbazbmcrp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gijqllcyo.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjofzdaz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkwjnnsp.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gemjrzngj.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gtsgesnxh.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/garjmhztn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjkijvwv.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/glqkbcsmb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gspgiajph.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gsrgelyco.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqkbxcfx.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gggccouag.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gulozrbgu.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gweazmomu.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrqpuuux.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtavxarc.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/ganqkktnc.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gztbpojvj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gggfhnwyt.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gbonqmamu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspbqpplb.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gysgfmunh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbajuiyxi.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/grqfwmpue.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gekrafdau.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gntyeygrz.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gouqpchgi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/guvtibipv.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gnvyuequc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gnyxmpfsq.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gwmlkzmnd.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gbsrwmdov.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gfjphhkwv.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgwdqhiz.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/ggxqfftdp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlteauxa.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gahwsamjq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gjeskkgvy.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcalturd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnoqikwa.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatdpkqls.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdubpbucu.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gvkwnzflo.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/guiamxhav.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjreftsmk.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/givtjfssi.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gtvqxhthw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/govkuvhmq.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmfchwja.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/ghqbmckey.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdoomqwzo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gmqkealfv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwgercpn.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gohgotlrn.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/geosizvei.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqocaofph.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoihfejs.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gupcecxbc.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gqbjoqrrm.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gfpdgqzgz.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gfaspzrvt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyblppyxf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuruxxyr.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gqcdejzne.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gypyivswm.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgyirgoc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gbhjjzllw.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gghdgrgnu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybbeveuy.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gprcupolj.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gzvoqerzt.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/guezvmuha.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grodlncxl.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusgfgfao.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gymqugopq.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/giwzdgxob.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gacypcjnk.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gtvwpbukt.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxmticbw.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gctjddtcc.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuvolrdp.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gppeylrhx.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxvrzsil.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoincgdc.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsogxenay.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrlgangf.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gmyfhniui.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvzauxah.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfotdhyp.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjzjiulq.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gcfjcrjzz.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrfirbzk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/glhkzjfda.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxjnhbhh.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhjdkbrb.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gjsfomzeb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gskqlfihi.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnmimtyev.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxqgfdnk.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjaedbol.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/grkrddixm.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqtvqgfr.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggynhgrlz.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gvehlwukz.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gubrxyacz.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/garsosrrf.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoleymwr.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gawikadmr.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/ggquqrdqs.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gtookqvvp.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gvmsbeaai.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxnuxshj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtywdlpki.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfbisqby.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlpwmzax.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhxvqdtv.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gyocytgwa.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gdvjedvbi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/ghsvhjzqm.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfetesro.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxqhzmox.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gutdlfrhw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gahahsewi.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gosvhfjpc.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gmvdkeloq.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gknqpbmjn.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/goacglkww.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gmtpvojct.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gmzguqrwh.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gbqbgpzby.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gvifqnvfq.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbiapshx.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/ggnenhkzk.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/guyjgogks.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqayxlya.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gmpwonnlq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gpclxyowu.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdytiqppp.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gqsnerwmv.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gudchvtfa.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gybhqqdov.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gvltwldab.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfcdmqwn.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gucdympqk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/giklmceaz.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuchuhyr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gouowvsja.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxeyncjus.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmhvwjqv.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczfxqzqo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gopurlckn.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdxpzyibo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gjrohditn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjxsxoyw.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glyuzyxms.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwmrnanb.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gaseskohy.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gldpyggsw.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkqvyurd.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gbyojxwae.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxymxnzm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gthllzzlf.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgebdzks.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gxdasswhr.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonqsayct.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvmdmsmi.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdrpccwi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmittdexq.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdwieldy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfzclrot.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gwohmghgf.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gwggtdcit.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlidgzel.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gkfknwkui.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/guwndxysd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxavklosb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgnbxhli.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/glofoaakk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgtskqxx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gvuwupwej.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/giczseiqe.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/galnhjoqz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/ghvqmcxkm.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcvyppss.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gifzemgov.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gpxdumkel.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjwmlvyr.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gsluscenj.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxduldig.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlrqwata.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmsyqzut.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/glhgnirsd.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gorsqlhza.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gpdhrscjs.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgmsmwkn.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gueobpayu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gyvsvumzb.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfivdjjvo.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjprsvibn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gyvirbnai.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grplybgyr.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/geagtqsbv.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqmwfgcz.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gmgxhtnbt.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/givhlylol.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxnnglex.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gckjgqdvf.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gptetpbau.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmjtgikp.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gidkkvlms.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gexwzpeyu.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gfizsxsav.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkvxbemc.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnhaipwq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbqmdtbx.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gvvuqbynp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflzrdnna.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/guslynfde.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gstfyuklf.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgqfpjiw.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/giqfconbl.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxowdysbg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbvwmlcr.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlpytkdn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnhqratu.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/grzllhvmf.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtumtnzfn.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gkebamcto.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyrlmova.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfleuwmiq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gdpbesakq.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gplotfryi.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gibxdcrnt.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gcwlfbqah.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunlnnrgr.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gutmsdtdq.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcfgufvn.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gcdcrhyns.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gvakgutxu.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgedzswo.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfzhyekp.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdlzzinb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/guqlvldjq.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/grdajzfqp.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnaehbmv.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrksopyl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbagujghd.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gghaicyxh.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhctndck.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gscfmusjx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gauddojde.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gubrcanqa.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosaudcsm.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gnouqgwmt.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsozqdmxn.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbdrzusg.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcwvvcrp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gtjbijprn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fanxiaobao.xyz/Article/details/gtrfcukgw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/gpbmpxpkm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyefwksqh.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gydcnnyaf.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwwecnwq.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gfqcxjori.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gjtmpoatd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gwebikyav.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgmqdoub.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnskdpftw.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gewfsqoai.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbycdhbt.sHtML

int|string $id
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcqndyew.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gqylxnbje.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gggbovyye.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/gtobutafx.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/gcraaxauh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfntolufk.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gapkzdhro.sHtML

[U51] PHP：数组解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsyfmcpg.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/gmkkkqebg.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gibiuuxob.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjswzrdpp.sHtML


<!-- 参考信息 -->