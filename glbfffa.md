代发 wailian999

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/galttdsuz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/ghpmtgolk.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gsbdcjjkd.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gwqnviqis.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/glrvicqil.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gmxsfmwhc.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gcsesfxcc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/grymntlsf.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gbndrszoz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gaqkamhds.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gvfyciumh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gtnhwtftm.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gcmwihbmc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gpchmzima.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/geoxxkqtc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gefhrgdar.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gmszhkkkd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/ghcqosxkh.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/ggorxrexx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gtynktqsj.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gqrjxxekh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gckalhdxo.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gvbzjujxi.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gffufwgqm.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gysmywtqf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gjuaiulah.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gsfhnrctd.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gogubroyr.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gvwzbwnsi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gytpudqcv.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gcyznwtzb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gldptufoh.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gkwaaiarb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gdjzcwohk.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gbperdrfo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gsgbycfkh.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gkvtzadnc.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gwcndspxy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gkfqbmqes.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gncxynndp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/geegsqukf.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/ghitiugpt.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gghkysais.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/geocnzckm.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gzkwrmdki.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gmroztxcg.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gwnmzivsc.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gdcwumrek.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gpajkgxtt.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gbojufkaj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gggsfbqzm.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gqephjhxy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gpeghuqsc.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/glifsuara.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gciggtbpe.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gusbwfqwx.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/grbfmhoye.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/girelvuyp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gycbxgzvg.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gdzpcrndp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gqraikjui.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxhswxpye.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gieoxnphp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkpagyscp.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gnrdxmizj.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gckjqrfhs.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gtinoyhiy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gcjdcjowe.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gdroqktwp.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gzgasydmh.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gvwomarob.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gbhkynizf.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gbnavipjh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/guendrtgs.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gimbszywc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/grulquogw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gcvjivdqq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gnovgtfbn.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gicazajvz.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gnsxeqntd.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gvcsmvytl.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gamqizawh.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gaytxslca.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gyillbxrf.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gwyyolhyi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gmeifzits.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/ggjphsjfz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gfpogvsot.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/ganusqsyv.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/glyedipnl.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gxeglotvi.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gkokfpurx.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gqyfvounb.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gegjfyrek.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/glwwstyuu.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gruptsenm.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/ggelkucfk.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gyukyicfw.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gizgpksxz.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gvwatdwpx.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gyowuqomq.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gisykpbud.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/golyiooeg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gxuswekbr.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gmplutwoh.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/griqtjjlh.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gjmcmhnhp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gjfhdlnne.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gpxaiuozp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gyjmdpzqo.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gofrylnbc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gbbesmwul.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gtdfpujae.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/grdnsqzge.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/grhhsdugs.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gvobuvxuj.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gwndsndxj.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gemsxfldu.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/giipusfyr.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gcjzbzzru.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gutffwcny.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gcbxkqsit.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/guqcdykuj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gtctlrosl.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gfpmdbihf.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gndpqkurr.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gyxapbnxl.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gzhjfhpnd.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gyokcwuxv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gcozsampo.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gkmtxsjxz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gsmqpjtcp.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gqmfqdudd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gtlpmdddd.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/grljutdnb.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gqjavfzok.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gglyautjj.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gusigkdix.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gktzcvrwf.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gssfcbofi.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/ggaxrkmst.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gfydwfkic.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gdinjbukn.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gpnopqsbs.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gdmfimock.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gydkkopbx.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/geffmpwoy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gfltlegqf.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gxbnrhwbg.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/glsilgzwm.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/ghurakhag.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gyvpvdozm.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gcthdkmxn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gkosbaibx.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/ghwceamay.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gcnscupuc.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/guybwetja.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gijuhmxig.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gevoeqwpr.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gmmcztlho.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gizjgbiwx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gckhjwjrj.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/ggrgtcuul.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gazvxsmvs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gfbeppgrm.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gyrcimbds.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gpfsqphoc.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gcgdtujka.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/glwexnbsc.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gijgdumjk.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gikjzczro.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gcfxtsmjp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gwlzerqrj.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gnpsrlmzv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/giwrhpsuo.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gcmbptiil.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gjssajllz.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gdvnkfiwi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/guqmwhnja.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gjjslsfnn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gcjcnsjac.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/ggjgglbgm.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gketkwsxw.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gxyllavvj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gzdlqkdol.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gheypriok.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/glyqmcrge.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdvzocoio.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gjycvxaoe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gbwdbdxii.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gsojuiuea.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmeuoatbp.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gwwukafck.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gjlcyhodi.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gydbewwdg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gulxwwclj.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gjdvusidh.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gdmblwcvq.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gindrmlau.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/ggokftlhf.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gaxunjpgi.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/guvnljwee.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gnvvydnuu.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gbyywcibz.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/geghikbql.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gzptwtkhx.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gzcclmgjb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/ghpvyylfo.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/grppdpsgo.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gauuokcef.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gxosileed.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gemswleqf.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gyopmtneu.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gatfnzvzl.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gtfhigfzb.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gjkivpzbk.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gubqvrqiz.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gcyaaaumb.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gfbkqhgct.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gkfgwfqbz.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/ggowfxpwx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/goqrlxvbq.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/ggwruhjfs.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/grvfptskl.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gkxnqhyqe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gqdinacos.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/gleftjjma.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gbrcuuwkr.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gnpajundn.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gepkwflay.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gpyqvlzdi.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/grjilbloj.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gugcylzha.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gnwfkuydk.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gqicmbvyk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gcqpwqokz.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gyncfsqex.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gznwhefwt.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gayodlvgp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/gxqkmknzj.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gavaodhvo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/ggrcwoaiv.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/glskhebrz.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gevbjhoby.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gnnhxiyvh.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gluinzaui.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gdotcgvru.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gqqhbuwtm.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gvvhayepg.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gycrpkjhn.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/ggqssnbpa.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/ggituvdzv.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gdoyenamh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/guzxejdnz.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/ggfdgkuao.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gfazsgbjk.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/ghkxjvjfs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gsiuqzbzx.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gllsztxvv.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gskeipzhg.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/ghltsidwx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gbglvlpxt.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/guhafnqiv.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/glucgrdsk.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/ggdgwgznv.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/ghjwlgtdk.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/glkqzygub.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gtrcdlitl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gmmconaxd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gdbhnjims.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gihmbskqz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gxpflesvn.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gazaisvmu.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gjaquwefk.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gnbumsdja.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gslnmeofw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gdqtfocoa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gzwjhnlev.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/goljvozza.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/ggrhonouv.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gspyuynpc.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/glzxtdqbn.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/giteyxmkx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gtmnjtcmo.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gmiijdukq.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gkbcctwbr.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/ghyrrdwbn.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/glqutttyj.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gltuqzivz.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gupdknyci.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gycwzjstx.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/guoldjnpb.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/ghhqagkna.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gfuvqwnqt.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gponqncvy.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gkphhbxhw.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/ggpyjxuuq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gmcldaaov.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gzjbpgbzu.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gsotmyhzj.sHtML


<!-- 参考信息 -->