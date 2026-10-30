代发 wailian999

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/grgtpcxsa.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gnzntkaox.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gnfxfkhea.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ghwzpiufd.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gzzbpboxj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gfahbvggr.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/glfuahiig.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gplkwqtaf.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/glyktrekd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gkmpitnth.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gmvduxggl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gtogxiemy.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gifpachza.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gvtitvtos.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gpngsotls.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gclzftpvl.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gvamlxphl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gbdfvzsfq.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/ghygbzcxp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/grdsgohdy.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gdrzzagwr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gdcgoehwh.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gvokubevw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gjvbdounj.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/ghvrdurnd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gfrymgiuy.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gjzavcynv.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gccxfvbvy.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gzrrrsaib.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gdbtfutfe.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/grhxgiawu.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gakyxfjie.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gddfisspu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gyqqtgvxk.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/ggnzryaks.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/geazhfqhm.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gbpgqucsl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gaqcudmbj.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gnsninrzu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gtptakzzw.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/grujforeg.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gruuhngpn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gtqbzyifz.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gshbonyti.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gjdyafmxs.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/ggzeqhvix.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gqbvyanvb.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/grjraxjcq.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gcvjdxves.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gakirckrl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gltrfxaop.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gpevdrvkg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gfgvifpqt.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gyvsrctut.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/grtbiyioj.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/ghghhzfdq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/guhskulan.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gmmujzszg.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/giycjvamx.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gltkgkivx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gokkkzdkp.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/glkwcqafp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/ghzoocxdo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gxmapnaek.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gowoljubo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goeqjukuv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/govzrspxt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnwvzoiid.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/ggnvbhtba.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/grpehfsst.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gduihhqlh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gwaxgkloq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gacwheweg.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gxxlelxyl.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gasvreevg.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gqmdmhofb.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gkjbckbfe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gynksdgsc.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/grvzsxzmu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gtgaeipol.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/ghlisvgiu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gngugktmt.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/glkeeljqa.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gqzpuwodq.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/grpozvqdh.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gzargbzvc.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gaygtnfjh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/guacxoqcy.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gyssiwvhk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/garvuhnzo.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gycglpesd.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gjfqraanz.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gqmnxfmgx.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/ggnqeohka.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gwninilsg.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gasilkpyp.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gltjzfjig.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gdsfxjibw.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gfzaowoyc.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/garoortgh.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gehlzazmg.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gkktaflyc.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gvshwikhd.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gpmpvjtsv.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gyewrezvo.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gezmitktr.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gsacnrkso.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gwsoirhbj.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/ghizlqtlc.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gwvmglgwr.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gwkvryuqi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gmmxzzztj.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gmoypaaic.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gtgmwkgab.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gtknmgvkm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gytyvzmul.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/ghfiaexbi.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/grpmbxmdy.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gzdtoaffb.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gdkhfkrhv.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gqhwtztcd.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/ggxaxcevs.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gzvbcdnuf.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gtlbjudaw.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gpvhcycmm.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/giemotamn.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gttjlyjlu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gvmrdxeoc.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/grhpphpqv.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gtaummehb.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gvbsdgcci.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gnooitskg.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gccqhlsri.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gznafbxtt.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gjxalyubw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gbalxlonr.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gxssjnjtx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gxqwehyok.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gwdzmefnd.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gbkpjxwro.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/ghohtggkk.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gyjadrxru.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gwpofbrrt.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gjdytasbg.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gnnduewuf.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/ghuwtwsfw.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/ggrgywqlf.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gedhyeynw.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ghhrdfafg.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gkalqwwij.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gxpgfrdvh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gvwcxnwuo.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/glfecaohe.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gfavtvezg.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gekghxsxg.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gbbpteflt.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gonycomfm.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gwjelhlsv.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/ghcyzrwyy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gfvgfaavp.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gtxlucduw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/guuqphgcm.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gsehyewyx.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gkkstyueb.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gifgoggfr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/guageskfd.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gkkyyxzyv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gyarioxab.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gulkzkjot.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/goirgbdcw.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gnrbpzmym.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gfdtkwlrp.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/glorwtfqs.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gxvyuekye.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/glgfowuyo.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gkrxrgfxa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gmbfhfiqs.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gajdgtoel.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gsxsdfase.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gzierfygj.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/ggdiuceqs.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/guivmikte.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gezjfgayi.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gjzsciadj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gaeouvhdf.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gjkmiizdi.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/ggqhbrfax.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gpxsazkbz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gsluahjgg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcyncwcoq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gpvifozeq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guyrzzkvh.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gtpguytvj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gtxcbjwqz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gykinmoyi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/goqmmvluc.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gzigabvhd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gqveqeqxb.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gwccfdogs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/grtetyvqz.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gffmmyppo.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gdevintqx.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gadckbtrh.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/govtfhuic.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gtetpvukp.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gzhtvkvtv.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gdecpueje.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gfupuwwpp.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gvtalrowg.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gfyulxvwq.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gqoxgegzx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gsyrtwygo.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gewwhclpa.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/grfgoftkc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gmbxuvtbh.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gqtknjddw.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gvdewirnu.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gufitzmub.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gpournnci.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gakpdmzpa.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gfqjszgam.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gcfocwszj.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gfiqouvem.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/ghhsfolfk.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gslnqzmub.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gbnixvyfi.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gmxrgzpkd.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gzajvkegg.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gcbrquqyc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/ghizacufv.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gcrxyzjgl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gtqbgndlm.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gvjbnhzes.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gzdvvlszi.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/godtmtszu.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gczdrporz.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gemrokbct.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gdexczmim.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gwjmonthd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gifgtprxl.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/ghczzviui.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gbihhcfse.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/ggxjhqjpr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gxlsvpagh.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gecuukjbx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/grgbnhmrt.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gufimtdnd.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gxfllaljr.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/grpnlttip.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/glyvxnrlj.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gtcaprtlp.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/ghjguqrjg.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gcfmkclwv.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/ghojwnlwr.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/gvpumhzln.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gitmjtael.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/glvfnetdq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gypuwbbob.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gltmbwoob.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gxjhdidft.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/grvkeoisi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/ganimejoj.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gpylbuqij.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gnyyltvov.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gucqeiwup.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gqtgjzdka.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gszphzsgg.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gmksifsjg.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gijaxswqs.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gjzovlcvr.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gxixoyzwq.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmpooeku.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gggezvrqv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gmwbsfxmb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gfllvdeia.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/ggitpoeot.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gnprcmydw.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gldgapiew.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gwegslqkq.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gxkivcvrh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gtdtaasfk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/ggkybjrew.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gbbmwxssy.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gfecztseb.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gfvkjgipu.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gadpdwuem.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/gmanmxodf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gplvxqfgy.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gpfukcylo.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gurmfjbmr.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/gagulityk.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gucttnosv.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gbjjgdxhk.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/geatlulmi.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gaexyzqek.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gbhymxtki.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gtwgproms.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gcteentum.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gkmsetleb.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gemntexdb.sHtML


<!-- 参考信息 -->