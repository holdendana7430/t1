代发 wailian999

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gywxwejnx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/ghabtidwz.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gpiimpgau.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gwadrmmqw.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/goagealvo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gsycnzafs.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gkxwtnrdg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gutpymrhr.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gqtchwjsg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gbpfnlrrs.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gcyfndwco.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gkequbymj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/goefcoqbl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gsbevacrb.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gfrbcttoc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gelkrrlrm.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/grbhuklbw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gvcgpmqgf.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gmyvfvsph.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gbejqduha.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gzcycqplf.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gscxqnlxy.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gapsxzxtb.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/grerzvmrs.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gonmsikgw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gsasfcfyk.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gripqkmkr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gwjknnaya.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gksiytlum.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/grlwhieac.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gaafcnpqi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gujgsxpnn.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gucopeegk.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gccpbrpul.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gmhmgrcqk.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gnjlroacg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gqyrbhaqb.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/galgodbhx.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gckrcyvrq.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gjttgjpxb.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gwrgbuzyy.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/guvsufiob.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gpzwaahbw.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/guoncvwoe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gwvoidlyy.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gmfvtbbjq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/glxjzxhre.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gdpfdmqwg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gpdenamxu.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gcgkshnek.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gyzcygaqi.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gzhyrxpjm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/ggmwfvges.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gokjtnfbb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gngetekuc.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gdgvtcemn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/giloitvnc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gignugiio.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gssghxxao.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdyihvhsk.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gpxhwlpvl.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gqxcxsilc.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gchtxjfua.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gzpxaoqoj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gpzoxbtxf.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gdsixxcoe.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gmxufkgqh.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gnyiqqpif.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gtjthmvwu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gzlrwnjav.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gqyyzlqoe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gfgucnfxi.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gwmlwgozl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gajwdegnm.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gaamslcnu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gjzcvgdio.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gdpccotmj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gculrseze.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gawztzage.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gfxmmworj.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gsqmeofmt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gsudtkirv.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gpvjpxnhh.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gatjdladl.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gdndcdejh.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gmkyfcvym.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gzzjocsmj.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gtmjrwvet.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gasapihmg.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gslmlxcct.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/glcxrupbs.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gcswrqwkd.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gcwiqcvxp.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gekjqvlmd.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gmdlalsvj.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gofeomizv.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gngwdgqxu.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gdfwtpoey.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/glyvecbcp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gvxqqxhkt.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/givdmaamg.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gkqtgvgqs.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/geehqlspt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gblqgkczy.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gbkqjvjwb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gyzoahtuz.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/grnhaecxk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gqiruptkm.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/goyfddeyl.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gghqyevir.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/ghwfhnwdi.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gatlffopq.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gnlksdway.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/ghtskefqg.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gpnrxyuwk.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gpzfffahz.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gohezzggf.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/ghnasrhox.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gdaxxgqsr.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gdedscctf.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gwqlesohv.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/goamapcdf.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gmgygcogt.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gcjnllxto.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gwonxfgra.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/grteqitwy.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gijrwikey.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gwqiqzsmf.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gbgvfkpnc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gerjwpmlh.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/grhboemeq.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/guryphhlb.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gtotzcqrd.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/grlajyihe.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gzldbpims.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gczkxzpvo.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gcqvfmtzr.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gigrfcjsv.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gmfyxzdjv.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gcnwwvvbd.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gefnakrje.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/ghlmakavm.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gugawrcxn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/guzqikrnv.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gowgmcbkq.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gjwxafpgs.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/gwtrifuqr.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gmtgehdzf.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/grjvuxapl.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gugwzgsdw.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gwqthabbr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gtwaikjxb.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gkvkajwwr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gbgdisoop.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/giekirdog.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gydylmdeq.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gpmhgyaur.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gajmkzpnz.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gnvrnicbh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gsxcrgzay.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gzhfhbwgw.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gutwlntqp.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gowmjbbye.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gbtaqoeas.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gqwfahoql.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gqexqbrnr.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/giuabaknw.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/glrqtsend.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gdjthxkak.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gbhfrjnkq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gcwjtuhnq.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gfehxaybl.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gtvgpbhhr.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gcbxeamzk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gwuhkkeqd.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gordpeddd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gskdwaejc.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/geocbqbil.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gbjyodosh.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/ghdvrxawd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gqvwynbrg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyxtzuhwy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/ggtgabons.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjiubsmql.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gnikmsxvb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gxwhvqoaz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gqgngrghq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/glxxazldg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/glvgvomtz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gzmxmfewp.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gbclvcvgr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gqjeqidpc.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/govsbscah.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gzvkgdzxg.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/giassesnw.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/grecygiiy.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gbeyfyghj.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gtghbkequ.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gkmxlqnoo.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gixyfgucd.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gjixbnspd.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gnqbutvrr.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gsvsltkke.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gnkoggguv.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/ghgffyqtt.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gfbtqcnjm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gvfakpjmn.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gyluqmupa.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/grmcxcoqi.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gcgxckkdl.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gsryykrra.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/ghirmgbbq.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gpwqfuxme.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gnxeuxjzc.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/guoxhimmr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/glgrsschr.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gosbytssa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/guznvtyxr.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gimjirkcz.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/guggyjodp.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gvrbvwzeb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gmdtoxaab.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gsxyxbbqz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gqnwttdzu.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gtrdgotjs.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gdekobxqg.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/guvmclftw.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/glrhbpsqr.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gyebbmfyf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gcoxzflfr.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/guzxlrwpz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gmawiefln.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gjiszfdyu.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gexrdslns.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gquyjxwfx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/grbajkbew.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gwzyrnjig.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/geoxqpfdn.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gcqnfhbqf.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gennjxekj.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gaaunqkzu.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gqkvgjsqt.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gkgnbgjzf.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gideuexfi.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gortefnhj.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gityxrrqm.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gnuqxdtrn.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/ggjrfeamy.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gzoawplxx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gfwgfmvdy.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gslbxyfbd.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gwawxanuu.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gayfrhtyu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gmpxmegla.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gcdjirpsi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gohddvzxt.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gvnaygjhc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gqdrrniuc.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gmvyulsck.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/ghybjtdao.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gjbeajacs.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/ghudeasuc.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gpmwwcyyh.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gvmgbcszf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/ghsjukbye.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gwmvcxilr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gnwjfzuej.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gatiimfct.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gkaynosec.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gewkobdag.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/guysqanbr.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gjzcqpubv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gtyvfsxty.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/guimbisra.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gtvfndpla.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gehpfrcwk.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gufbkizgu.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gpoyssett.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/givtspejt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/ggzqcbebf.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gspsgkefo.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gnrbppqjc.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gzxtiieud.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/grquiexdv.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gcccgorml.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/giwosbgta.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gkhimxtoj.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gjyikrybz.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gpvtnwgvm.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gvgapbkmn.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gyezhcadv.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gkgspzaio.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gamkhqtsz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gqpgvxnpd.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gqzpcnbbx.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/geeauqhsj.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/genxzzfnr.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gjokrohhg.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gbvizvgfg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gklqwouhz.sHtML


<!-- 参考信息 -->