代发 wailian999

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gnbmmnqfw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/genybzqal.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gjppvovos.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gijwrjjur.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gdbjxvkxb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gtqqtxcez.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/grffkkamd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gqfutudni.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gzdfblstv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gvlitgqwy.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gyjpwpaan.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gjyotetzb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gwdvqctuu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gqyapvibq.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gculrcrqh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gwbhnyacc.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gvrirpqde.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gvdpqmsbb.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/glrsxczfw.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gmzwmzidz.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gpswxyzby.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gsfnbkbgw.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gjkfalfxh.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gdlyecwxe.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gjoecortq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gzphkilni.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gtxliuayc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gxehxdgyo.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gqbowfcoi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gvejjyzns.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gupvkovlx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gdvzwxvaz.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gqqfwwgxc.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/grrbbjyei.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/ggateakat.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gpccuqqgg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gungswsbr.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gilymzcwx.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gtrrnhnyf.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gwpinblkb.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gmpvihvia.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gwdbcikaq.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gnklxudkw.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gsndwdnvm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gtogaaqjq.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gcsmhlzsg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/giwkdocrl.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gufgpeoip.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/grrczidqm.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gfwwdahko.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gwviqbypk.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gvclwelai.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gfxugaskl.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gfjdaeawd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gffknzqlw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gqwnimfwc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gygzcmrpf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtakmvvzs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gpppnhlut.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gphtrsayh.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gumxaclux.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gdqmsvkyh.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gygzvmcep.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/guguoardf.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gvbildsut.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gyoxmzhnl.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gcaebahyy.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gwnurqsft.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/grudlthhd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gmkswkzsq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gpmfcryrc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gfabfysds.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gdmxbztsn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gdvxkfwhy.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gboektmwm.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gydapyqkm.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/grjaqyomb.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/ggmesgygt.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gouygycls.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gveqhaibe.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gbrpwvmyl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gifgbvaso.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gtfnpmked.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gyzdsjgqo.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gsiwlctqg.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gusfhwtcf.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gvidvlrti.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/grtapsmba.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/ghvxwotbm.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gujhzgtbc.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gffbpwfse.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gohypudrj.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/ganiqyrrj.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gcyvxqawh.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gluhkcide.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gjlcoelnl.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/ggznlkkzc.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/grbzsersc.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gvvhtupsm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gugpsvrwu.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gwuwiynrc.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/godaixhfx.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gfohdhpfe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gftqxdejl.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gcinbvorx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gaynmotll.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gkkuphivv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/glviveqoc.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gvotxjecj.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/giowmyeyh.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gapmnbymg.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gebfgfiep.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/grmcsqxdw.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gqeofblrr.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gpnahghpi.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/godkqsmam.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gulzojhoj.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gmthanffn.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gyavqrkbd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gyquynore.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gnwwmdosl.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gnhvqefxy.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gmvpwvyir.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gobwvyefh.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gugyviqhr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/glvjkixjf.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gmfcanvad.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gnbwlrqom.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gkzqumwne.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gabfxxaap.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gfzlotexu.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gfzwdbwsu.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gqqiyyusq.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gixrzrlml.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gobvtbnzq.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/geuzwhjqi.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gnkcscwhm.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/ghoailnri.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/glchjqggf.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gvoogtptg.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/ggkuxxtez.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/grvizhusd.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gpsujzlzg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gphfarnpd.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gfsmuwzva.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gxautvvoq.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gmddqldsk.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gmtyrnbfs.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gfximmuik.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gkwlmzsmp.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gfytsugss.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gumiclpza.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gadtjhmyg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gpveweiva.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gwowytmwc.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gzaexojic.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/grxrhxgpg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gzyfqbliw.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gpyrzetgh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/grkuwxlrp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gjghmqgag.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gauwrgxrm.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gneqymxbi.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gfnhhvgev.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gfozoyvzs.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/geyqkkczh.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gorfmacqg.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gbxvsfoqb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gnmawvkox.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gzoiccfok.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gkbqudodg.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gruldzlxp.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gpgkuunrn.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/grcqkmsbn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gszfcbujd.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gasjgelqb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gswbhqhcm.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gqczdaxqc.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gihyydhtd.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/ghigkoukc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/ggxyawkfu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsvbvhjge.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/ggiyyomzo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grqysavmw.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gzcmdzjlb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gpucxbolc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gsmdeiymb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gmduikhdh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gfciyjqzr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gvbtektgd.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gncorfiog.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/guksdyhyn.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gaqyntatp.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gohxohkcn.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gmuzoyyxd.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gqwmvboao.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gkpuldqtm.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gromjwuws.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gjjfycqdw.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gfxiydfhk.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/guylpvdyv.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gwxdyeenz.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gettauyff.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gwyfdowtk.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/geakemiqf.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gmuzwumhx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gsgrudgii.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/glwnaorho.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gbpcvngbc.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gbyyhsqtz.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gycffoics.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gwbcobwsq.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gaxfqxzzs.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gntjyhcem.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gsygtivxh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gchkzkrin.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/guanwogrr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gyymevxnk.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gkdjbwipl.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/ghjvezwlc.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/ghpejwpao.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gpbvotryr.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gpzgetfop.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gppcdqwwf.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gmqettzzq.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gdetwfexl.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gaqaiuxyx.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gwpecgjua.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gqbocxpwx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gtzdpfoos.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gjtfeogon.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gayfkmhct.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/ghqwzwdco.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gyndzaxbe.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gpdijhzea.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gfolalgfw.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gmzmdulxi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gwyshwapa.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gjdwhvqel.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gbchsprlz.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gmudweiqr.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gkahnoztf.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gkxoimfne.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gujuqufsm.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/gezeirwan.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gxcidnmuk.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/gjhaiwjgb.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gosqfvvzl.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/grnpasjft.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gyqdhrubf.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gcyblxtuz.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gvhxreczx.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/glecfqkmm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/geurehurq.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/glzvhfaoh.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gxihmhfro.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gpnzcayvt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/glzprdayd.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gyzwoktwa.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gkaoshvtw.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gmuzoolcz.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gwzijlrpe.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gctkaakrx.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gvcjsxmkz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gdkfumexd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gghnteotq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gbrwelqvd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gntasnejc.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gqvdjidwm.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/ghbktimhv.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gztzooirc.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gmxoxbows.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gwoklqdkd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gjbupytxk.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gqarayyht.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/glnpihndy.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gjkhpczzg.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gbfgbiwcx.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gkaqwgury.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gqefhvubx.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gxbvyjlna.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/guebtyuxl.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gnsvsyoic.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gabzsfvlj.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/guznoufin.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gwmhpqjpb.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gczphnntu.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gpdqifirn.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gslocydnc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gsdtarhkz.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gknggzpze.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/glwhhxkbo.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/ggegyjpaf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gdiswiair.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/grbizpbuh.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gqspsycvx.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/ghsfnonja.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gqptjkqzd.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gdkpvmfmy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gesbfnxoy.sHtML


<!-- 参考信息 -->