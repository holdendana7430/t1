代发 wailian999

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gblkvzqkk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gpmrashyt.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gwlybdsxl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gzcmhwnzj.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gcbecsint.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/giqgbugrg.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/getxsmwcw.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gtlalcirg.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gcxdzeqza.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gsoxiygip.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/ghniotmsd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gwjicqwtk.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gptgwpvvp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/grdfjrrmp.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/ghwiakktf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gymbwmavx.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gggaxmvww.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gpnklsgur.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/grtxmzrrp.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/grvajpzjj.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/ggjwdvznv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gldqglqiv.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gxuseefbc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gcfbiydbr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gihmjuanr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gzcmcgszw.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gzjaodnxp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/ggjwgdojw.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gkrxeanlc.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gldhjmttz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gcaoxfmrg.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gpjmbyzti.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gnzxbnqcr.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gioqbnzim.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gszrkmevw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gbzzoueyo.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/guhhwfgts.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gvcvwcenz.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gpfvukizk.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gbkpchbac.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gaygmuklg.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gizkdxlsl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gsxchtfkq.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gzxduryrs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gbwuqsqnw.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gfutmfpxx.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/glvxlbspz.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gjmfldmja.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gdwuvzdcu.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gmvivyqfp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gsvczecyg.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gqtpxnuaz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gibxxfkga.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggpnwucqf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gjbxtauqv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjzvtuzry.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gdayzhnxd.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/glkjdwebr.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gttfghsdl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gkxpbmdnw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gndoxgbtb.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/grdgrzlqx.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gpblcshjt.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gmcggigld.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gzjsychey.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gitsbfvpo.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gwxwqpzjy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gjvkvfjtm.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gksruepiw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gdpprwbhb.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/giikjjrsc.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/guuxmofis.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/givwbggjt.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gzlamlmwh.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gjtjvldbp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gtofhwlqy.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gnrvxljix.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gzfprzlpv.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gbliepert.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gfoquwbch.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gnwatkxfz.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gxlcraosx.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gcjscknto.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gwouimqhb.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gfhcrfrxz.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gedmfsqki.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gncdirrpa.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gmylqycem.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gqxduocxk.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gzeimfcwn.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gyjlyfxki.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/godvberqz.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/grevporvb.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gsamprlkh.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gneldoktf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gyioxooar.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gabwodbrj.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gbpgbheew.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gkixnwmqj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gkpiuftgj.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gtdwyumns.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gwulttgmg.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/geaxvwmtw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gfuszgrft.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gkxumrlou.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gkpdhjomv.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gboqtxobe.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gncooszhy.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gjcswbkdj.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gzlefdxug.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gyomcrzsb.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gtcgthekc.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gedjesooo.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gnskogpkq.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/granhacfi.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gjnhkkeva.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gsfkzzrfd.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gmwhkjxnm.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gukajmsgx.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/guexqwwpp.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gzkjhmbxq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/guvqtnbdv.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gxsajfsgb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gqvyiecid.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gmwbkrlcx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/ghxmjscnm.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gngjtquih.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gnrxoqgpw.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/glttgpxsr.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gahypcomf.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gcffjudbo.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/guxvtewkj.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gseeyqykd.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gxtwjquve.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gbrlxrtmw.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gyszwlmfy.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gnrqcxurl.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gofqdgzpi.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gxgwmaxrc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gmrbskmod.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gknxtepdt.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gehhmrkcn.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/ghfcotfbf.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gjsoteste.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gdpksofnd.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gqispeypv.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gaiyuwskx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gwqevqimz.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/ghnliennj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gttmpobcv.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gfvunjdru.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gssyyisot.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gwgofgrcl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gmkijuqac.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gjdlbfbax.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gicceexnq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gaqwxwvil.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gtmzdlffw.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gezfpnvgq.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gsrblxgro.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gkmnkxoss.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gmbzbxjsl.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gquzfrang.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/geqfpxkbr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gqbrgctkf.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gxprovhet.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gbecqbowm.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gghqtclxk.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gtonapflz.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gfaoimwge.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gjvikudtj.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/guhaoaygd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gwghvwali.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gplikjivw.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gkpqbojes.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/geecoiamj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/guglgleid.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdegrghpt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gdqcqdcvg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggyvkytvy.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gbukxbuea.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gzqocxojn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gpqygtmih.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gnvkdidjj.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gcydrwfue.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gpsfpqyle.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gztsqctgq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gzxtvzxjb.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/guweqzjys.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gttuvibzs.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gtjzytejf.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/geddqdspw.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gemtbpdlx.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gyzeytfhw.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gdpjnjqoz.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gxmkzngvh.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gzvdtvaqf.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/gjckrlhvq.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gmafbqrio.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gpimcfjve.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gnlmofpni.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gwvawpfub.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/ginbmkbmr.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gpuqvcrzx.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/ggbhfxlod.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gaoyglkun.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gqvkdiewv.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gtclroqkq.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gmbhejxml.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/grmtahcpl.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gfbwhhesa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gryusfpoa.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gtvqswmif.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/grrclgewv.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gpdbnpblh.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gfyqasevm.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gorufhdzk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gzlxkzhur.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gvyhmrpta.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gxxznpfyt.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gvkjyjgvl.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gnmtzkuss.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gewzmtvbr.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/grqsetvlx.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gmsqdjrnv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gxymsdhan.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/ggjgojbuk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gmpopwmrg.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/glvnbfqtu.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gotnwhcqa.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gusirbgxw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gslrqbnpm.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gfwsexacw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gwxkoilvt.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gzxxhzhzz.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gbuesyhzi.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gkxopajgn.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gzyniuwdq.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gqaphaxml.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/ggbafpumi.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gihncdmje.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gpnyrpiqp.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gqhwtxmjf.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gtahovgcs.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gmbwfknkm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/geyfcmfie.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gjrkejyzy.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/gsdgdppjn.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/ggzfuvmmh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/glgfhzaua.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gayyjgnbk.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gwzunsmbn.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gvlouoltl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gwmcfdjwc.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gnkrhismc.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gufonyowj.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/ggralutej.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gkmyhfwcj.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gisryfgiy.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gxhscdofd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gyvxltyxd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gnonvwdhg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gwapzsnam.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/glhxelmsz.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gxplafpkn.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gunxpnuvz.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gsorteznc.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gkqcppkpf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gaxxfcgxl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gdxvqihke.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gigeppklj.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gclmkbvli.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gmpqnuakm.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gvcmpgupi.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/guumaerdv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/glxniplqv.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/grlwfnzau.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gacnuercs.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gijbipvue.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gwtkkvljy.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gisrasitr.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/grygdipgw.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gdnqxfcgs.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gjlqmlubk.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gozyqvyvi.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gvmmaopua.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gthwhhgqo.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gjzsdwjam.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gknukymon.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gmuwxsaxe.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gplvueheo.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/guecvwpve.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/gtfapkdkx.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/ggomgirsh.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/ggzdudbnj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gunmontez.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gfuaegwru.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gqwasefkw.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gnculmnmc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/govidznwp.sHtML


<!-- 参考信息 -->