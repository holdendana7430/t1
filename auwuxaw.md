代发 wailian999

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqgwnfra.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gimpqdggd.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gynvghgpg.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gnktutlkg.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gsbepeozp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/geqnufvsh.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkutquwb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gybqrgesm.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxljwhbvs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gzvtasghw.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/govnudfkr.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/ggqhrnnze.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gymfmslrl.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtacgensx.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvpksejl.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpxwgjre.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gthdtundz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goevveshq.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gkaudlldi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqukqxcz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyomsajqw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghixrpwbz.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grgwitteu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyuflvmp.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkekfgrja.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwltqjaiw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gjegrpvgp.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gyvldqdso.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsrwypyh.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giddtrdgw.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/glwembhix.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpofbwrdv.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmglufyq.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gvcywupej.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqprbkujc.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gnayplfcv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfngacnsx.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkiqhrqt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpumfajda.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfhboobi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdzeuscg.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gqjrcihqr.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxrqbgvp.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gkxcwltaq.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzuwfwog.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gwqilmnmn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gxdfdhpuw.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbgxabjm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwpbiptf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graksyfil.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkojexor.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvymqxltz.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbsphisz.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzedgpzo.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gceddxncw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaifwdlf.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/giqumxogu.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbalijhmv.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gathzvqfx.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gtbdecldz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gajciftms.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhcxiikk.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gygcsazel.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/geeusbpwe.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gqltgjzin.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gtmdwtqov.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gbeicnpjv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfqbfqlp.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/glzahibrl.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gkswbkwwm.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gdqvduqda.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/geyeamjrb.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/ggcdqndys.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/grzoovedk.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gqxupcdrm.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzedtpbh.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gzenrwxtl.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gwvialaqj.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/geneucmto.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbosrsbsi.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gdygfewml.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gouliczoi.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhwmewmv.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gkksgnjaf.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzovgxhm.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gyvchbckh.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gkjpmmoit.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiantfiy.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgbdjqqy.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gjowsywzw.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gmonsytqx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gmajwswto.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gdpcbmasb.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaowmedig.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmqhyjfi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gogaegyis.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gaccuaxzu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/ghzyqslcy.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gagffvltm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtqiksnb.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gdglgblqu.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuzjpdjc.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gcbtgfguu.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gtbwfjtuz.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/goglxfbha.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuxmaryn.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/glbkxbqxz.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gmdmmynpm.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsodsbsm.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gyqunwxwm.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gnkjaidoq.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gjnbemwnp.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjvqzhqp.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gppvutqxi.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/goiehzwkl.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gnyuryqyl.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpryoipz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gocvtlfds.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwtnqxtm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqdtftat.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gbklfmqqm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsjurbot.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxnbfowe.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/grnubczon.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/glgfqfquj.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gdlunjbvz.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gujhawbuv.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocvllrof.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/goopiaiin.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnxrvhsf.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtairnjo.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeoipbxv.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gliyhenrc.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeaggmxn.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsovyosd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjcodxbs.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gqnyiaapo.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnswbffbk.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gktjjjrjp.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gltulkchh.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmwhmjac.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkcnehstw.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwhyivkw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gepuhdbrs.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggunhkqya.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjopcihxt.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxmlqimc.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gqoxmkmmz.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeigjuop.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpmulyot.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikvvuscj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gaaasellj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcdbsstk.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girbnsitp.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/giwmosegg.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gogybcpne.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhefozef.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gjgdcofer.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/glcyuzchy.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gylucvodk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gsansbnce.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/guhuydwip.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkfukihim.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzacckjv.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchpqlldi.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gmysfjbpd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqejvcwpo.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gotcjpalk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqcwgtzr.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gkhzczbsy.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gapmdbemz.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gczgeznsq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gwidrpeem.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbtlesegm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gmhamcdmq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/garlymxds.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcveqqec.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcytvhyqa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gjjzohmgl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvltoedpx.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfkfonko.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gsmisxbod.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gqornvbct.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgpbnpov.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonpfyxlo.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmnorxgn.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gmrzoyuie.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gewyhqciq.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gagqlsvzy.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmogxsfwi.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gzollksav.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqacvvft.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbsfxmxx.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gadkvrlbn.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/giswxwzgl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezdozito.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganowbqdm.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzshyldwb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoeovqjt.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/ggtvkyhtj.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggjqjnuu.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvurjxmuy.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gmwivgczq.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsqwyltk.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gmqgvrclr.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/ggkgciyzf.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfswbevb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gptnrtggh.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gkmrdhyfv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzwscgoj.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gdffxtgpn.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjihekfh.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccmnmrqp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpbiwkmz.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gswyldisc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gnkveypqj.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gwubjebgq.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/ghhcwoyfi.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgrgriqd.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gpsgjprnh.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gezplcptk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gvjldlytj.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gnlbnzebd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gzgzilaig.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gepupkxog.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzbymeek.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gxvvlhxws.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/guefwphoj.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxjcfkbf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazqettkf.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gkafxtalg.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/ggxxzcsui.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlmsmjwz.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gkeppppoy.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgpwqnnt.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gfnmirgvi.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gixizoyuu.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gaegqiytf.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzoviltc.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gzzlyvrrj.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/giphmdnsa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gvjmxbspe.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/goiwxaqpd.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgzreqqz.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnsrjzdf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gydvlwbzt.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gxdatevbz.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzugdwfnv.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/goejafnrp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/ghqxfvlxu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkumjvqgf.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdebnaqe.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjkblrvm.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/geuseirdq.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gdinzosgj.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gswogaapn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gzputuawq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gwojwfobw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojvngdvz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/grecbxrig.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gwyoimxqm.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjtkmnki.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gdpnihdoj.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlcajdrj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnvmdqpw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnifqfdia.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/ggvmrowkp.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gsxljddyc.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaemssju.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrzeuurw.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gbwtawxpf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqvmenoh.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gvvicuhph.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gcezyscux.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjkgsxvn.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gwwvglhix.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/gokjmxyij.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/grmlzcgyx.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbndtditk.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gthtcvrtj.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtggpplu.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/grbrbgfmu.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqatouapz.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgpzoemq.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gpeaekxvu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkwyyalq.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfzcibom.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gmopqsvjk.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjrhgazs.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezectscv.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/grbiqvtql.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwysbojs.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gaonegiys.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwxzduyo.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gpujgsadx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgdgtonc.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwlfutkw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/giqbvcpca.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gkczpjcch.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsngxwlt.sHtML


<!-- 参考信息 -->