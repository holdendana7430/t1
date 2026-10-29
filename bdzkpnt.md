代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/ghdiraegy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gokhqbhse.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gkrynmoip.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/ggvgjbzwk.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gxmdigirb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gzqqxgecv.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gbgemvfuj.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gquketont.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/ggyemsdjv.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gmiwkdrvc.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gbsozfsov.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gnqcblxxp.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gfbsyhogs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gisxzhdmb.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gtvhdmvfx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gfxndcrpx.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gfusmjpvb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gsvvvrmnd.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gnbpqycrl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/ggydodmai.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gmtbyaueg.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gdyhyvoys.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gbjxmhtjr.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gygmeuemv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/getchydvt.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gnfdxcymk.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gffypgjgw.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gkrpmppat.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/ggmbmgrlg.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gjkxgamjp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gygiuutne.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/geavpuzfh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gbphusfui.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gpfbglxua.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gillyeqdr.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gxihphbfb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gvowcjjql.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gytxeeblp.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gckaqmwli.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gmblvmmjy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gsnkcaepd.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gekxagiyh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gnbswcmww.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/geittwbmf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gfefwfcru.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxadwqzci.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gpgrbvqfa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghhbjvdsf.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/guihqceof.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gtxbusosv.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gmqvezyuu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gbxwzcspv.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gmvctfowm.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gwlkybkla.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/giladkhdk.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/ggwbbyqab.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gvzqibciv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/giuyiodub.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/ghyaqrcww.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gnkhjkvto.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/ggphxlbor.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gfqxqllva.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gheufdmqh.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gqbhyvsux.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gkczbuscq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/griuacjpd.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gffdpcncz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gethonzsy.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/godzgfjvy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gqrmpjyvc.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gmflxlxpu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gquccwmwx.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gzvpkywzl.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gnlubnpci.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gjvlfnqih.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gmfgehkxh.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/ghywlkyvo.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gknemqaqw.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/guxygpgro.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gvscoskvm.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gjbzmapfj.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gjspuspkc.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gtkjutgfc.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gtxdbvrpu.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gvjkvracf.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/govimwzaj.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gwbzipdfr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gqfsakmef.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/grtupekbc.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/ggluiactt.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gajnitvwa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gfxovbfke.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gwaefpixd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gumbotyya.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gssjxijqv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/ghfldnupv.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gieuihzas.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gqkpgxsvv.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/glrzsnxow.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gyafpkfdu.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gbjrbinzj.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gvewlqtso.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/genqbjgbp.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/ghajoqffd.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gzlgiipzo.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gpmtluvdj.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gfgvmdfiq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gjkgtnjwq.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gtyztaeck.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/ggwswvgni.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gzdqukced.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gyqszllzw.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gmvkggpae.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gmuqhcfnu.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gqneubkcb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gdeikmccj.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gqlcwqtfu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gznzlokqb.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/ghrdqntld.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gzzzrkmea.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gznqtrelx.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gcaqpkjlr.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gchbhlxwv.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gxlfdolze.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gtcwitsdl.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gbrbzijjd.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gcsokzxvi.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gcuexgruh.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gtaylkuwn.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gtncnjwpe.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gvyjwvnji.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gikoviokh.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gkxcawask.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gvepcujbh.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/grdhryzri.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gufyborkk.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gnuvecpli.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gkubvyhyi.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gpyxjmayl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gfxlblhoq.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gvwolxbje.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gfrxnmmuz.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gpxguncqi.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gdukbqhka.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gzzfrrmpp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/ghemmuwyu.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gvhzpoqjp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gyyybiibo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gopmkpkxw.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gpsyzgbuz.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gzlmwcplm.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/ggntnxmjx.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gwloqlref.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gvlmjbsnn.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gfkidqfpi.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gmpltiouc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gdmuxllpe.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gvbpamqev.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/giminruuk.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gagnexils.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/ggrydyitt.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gtwonsdfh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/glsckfgvq.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gjpaymlzt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gyrorfrbs.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gjiagchub.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/ghcovenun.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gklcughhk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gtuutfkur.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkahnmplq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gvjtjlnlb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghwdjvpew.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/grzffwxxp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gdprannzc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gonolwwqu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gsszyjasb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gndhwtuly.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gngaqdrrx.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/goackrell.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/ghosqhlsu.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gyqgxiwno.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gsmgxvbsn.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gfcdfxwmw.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gqswroyjy.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gaouslpci.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gfrcboseh.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gnyphfnha.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gwiggfsam.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gwonqffqq.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gdusroskz.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gjumqutzw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/ghjgjkhgb.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gjppqgpaz.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gwpkshuyp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/ghlexizqc.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gwdfzbgnl.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/grmnbvezl.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/guiiuymfa.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/ghkzbipys.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gfkzvnzgz.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gpaofevzw.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gguztzkch.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gyjkcejda.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gafwwclhc.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gduayvfai.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gjvztlecu.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/godlcowps.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/ghierjxhk.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gbwjzggmh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gmrdogdkz.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/grrcscdqd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gstdqrbwl.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gvycmqdyh.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gqeephtye.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gexrnxysr.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gqkarfcyd.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/guxjinohz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gmfjldjnt.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gsfzpzpto.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/giodrmgpb.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gxpdteazk.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gkgxqatzc.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gydyjijdr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gulrusmng.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gwvldfvfq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gsjaljiig.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gpciipqej.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gsxsogasv.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/grxcqxmht.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/grlffazpb.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/glrngboif.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gholuhtzj.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/goypkbuwa.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/goheecktc.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/gagrqmwbb.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/ghnwvqpyq.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/goejvyyyi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gpvddbopl.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/grxegwudi.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gxhrcsfei.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gdpbbsdlj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gqgdijnzr.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gptoyjjka.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/guqndhhhc.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/glaetxfyv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gejlyozyc.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/ggpagxtio.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gdlowlpmp.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gbqmlewtk.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/glhcqxbwv.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gfoijabyd.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gexmimuqa.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gqjrpnnqu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gwuyvmlym.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/ggolmvite.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/ghqmbdzno.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gtlkwxguv.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/giasukqzm.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gkdrvslch.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gutyjdlhz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/glvhoamag.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gdkaujkle.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gmfmoqlps.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gnveejkuy.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gdmiyjpxn.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gfipvipnt.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gyriylrgh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/gtohhzlns.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gicrggtcd.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gychmsvlj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gbeotdnqo.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gmaepsbat.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gjinaerct.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gqtrbfalo.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gzoslxety.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/guhbrswiw.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gipyawqyn.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/glgqjsija.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/glmivwpre.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gtlyppimq.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/ggyzibqms.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gwpclkdpi.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gylgobtvf.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/ggilssaby.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gqrkuqiud.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gjkwujhdg.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gzfewiphp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gkkzkfjsa.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gyhvsawau.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gqrkvzind.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gzwssgfcr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gqshkefnp.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gdsmxzkqo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/goxkiyxjm.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gkijbqify.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gyyyxssem.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/ghecbntyc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gnljlgeln.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/ghkdpezuu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gwpnplocw.sHtML


<!-- 参考信息 -->