代发 wailian999

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyvqfxoh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgeqdcvb.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrhfeufl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/glqphxlsq.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/grfkzrisx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkxabrdh.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhqewluk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gypwukpyf.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gxhkrfrcp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gziudyexr.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywfmfqmr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrudupim.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzexzonlw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gwtowngep.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqfxykprt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmnjzwmv.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gmheatscl.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gomuadjyk.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstirmdat.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpknkwmvm.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gceduoknf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gosaeellq.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrlvqbva.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glitwyjvy.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ghjahkueh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqmwofuca.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxhxkqpr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjiylfuj.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyqgmtir.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/geqtvshcs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrrpwtwe.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gkpngmcnz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumjhtgyu.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnusjcrzm.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/glszntolt.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gohvgzhmm.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsuuzleo.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/glnyshglf.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmniawib.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gjpqyfcxq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gsmnuzszo.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpozqsce.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojrbdgqg.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gsyxqdsoo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gufsshnkq.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/ggpfxcqbi.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gbklnaxeu.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gjwvihqln.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmwrdrlx.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gbddvrbfs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gvigpvhph.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gzcpmgaph.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuxwjsiv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqsesvbo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/ghyuqlbxh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfoyyijt.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhmkvcqw.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwjhjdyd.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzcpjhda.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gmomtexms.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gmvtamlja.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxaoyvvr.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseqpwpnt.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gyilzkvcr.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjuqngzh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmtmhxsx.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gbtaojlbe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gobbhrgsm.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsckvgzp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoecefhi.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdrlqkqx.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gooslggfc.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/ggoirqipl.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdskdcyu.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gjuemgjdp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrltvhsc.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/greuotfeh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gnqyfejsf.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwjavuuu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfugixsmr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guaulofku.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gasdnjdfy.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gxrdyvrnl.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gxihbdvgz.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqqqclxw.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/guwxvyfwb.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkcnxhdx.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbkgogca.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtklyuzrg.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgdttlxi.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmjtpvcl.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/glmvvwjjh.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gxpyrajaa.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkglsxmcv.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/ghadxxzci.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhgexbqd.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/guguoumkr.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkxfdwyt.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbgrhebf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/giqfpwfaj.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmojkdse.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqqlverp.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gmojcquyt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glszvtcld.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gvntarasa.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvqwqfyi.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/geuluzrwn.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gecbmkmvl.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gutuzfnby.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gqrxswxpi.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gbbrqobuy.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/glbytchpu.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjcvnwlm.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagxjgkzd.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuxyfrsh.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gufqkpyhu.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gtznbbodg.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzaerlnzk.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/ggsowshrx.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/grmlpdygr.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/girbitqld.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtbldxzv.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gkwxqknlq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gbpqccrbs.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gaedawuvt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gfumqszdi.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghtlbqbtf.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnugpxkr.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtnksdjd.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gkcecuxrf.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdrlsmjo.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gzufqocbk.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahnmbmxv.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkptjovoq.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaehmhqr.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gxqbvutew.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ggkwxabxz.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqvchatk.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggskpneah.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gellworre.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gydvonuql.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqondsktq.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcentkqnx.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzvrbvnz.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gdymazwwt.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpknxencf.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnbrziyc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gchdyenda.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gqakkkvfn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guciwkjzs.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkapgzqj.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjishtnxs.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpdvmeeb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/glmectoum.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzetnpblv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpzrruzp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkdkbceyg.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gykotkuup.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxqsvvbk.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqlzrgzc.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfejxjcg.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/godfyvitz.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/giumnqhnm.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhholnsb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gcsohhnru.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gceusfdux.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gwyltgwyy.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gloshntpv.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbvgqpwi.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbgdrucw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gldzuqxtz.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gvolicygy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuxcgrld.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsmhaphc.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gknpiecgq.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvdtuena.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlsaniuy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbhklgcd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqmpyorv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grxqbqdzb.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gythjhayw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gihehjxlj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gsxdqogls.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqypdtlpo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndcrhacq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnririguu.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptdohrrr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/glkubgilw.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpksifgrq.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqwxxoxt.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdzhpnia.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmachsrf.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gntoropcd.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvrekvxq.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gxauhgdhw.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/gmnewpyfu.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gigfnlhlb.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gtdplcxdr.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gmpqhacbq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsghyzidv.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/giahlzjxw.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsfdgjbf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuhdvnnz.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gpbnjiolo.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkdoeiwd.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goeeqayhu.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gnidacgmf.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gqduzjwnv.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjhcdtvz.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/guizwylxt.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohcyjwub.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/grovbwdsw.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gamazvsgd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/goispjdsn.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gozvxsuxq.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/grihjknus.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtptktkha.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geitrmwkq.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gvrysorrt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/glkoysord.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldxajnri.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gjtbhuoix.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gldoknljx.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaixurte.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geobdoqdy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/glcrzyuty.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkusdisqr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/goeuualml.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gzepmcsdn.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlzkafxl.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gjutudkew.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gmylcjhbz.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvbrbybf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gbktrtnry.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/ggzxxvriw.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gosbhzfbe.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/ginyaxkpo.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gtpfiqiar.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxhslflr.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gqxlyloef.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwenuquj.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/grtmeavhq.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girozjhhu.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gygbfhzkt.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgqjefww.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/giohxzpjr.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gkhqrzpdk.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnujmwufx.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtbumlch.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqkajwjb.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnbuwabu.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/grscapzlp.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gafviwuao.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/giubbqrye.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gfxhunizc.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzdodcvp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqinkpluc.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgdruyjr.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/grqsbaygf.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhzpptzx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/ghffucmmx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdgqhzne.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrmssrig.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gctrdxfbt.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gdpslqrzn.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfycnjae.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gpcjjjdbn.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwubzclll.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhbzroru.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grmauvynt.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgnonbwm.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gbaqcjkuq.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giceuhavk.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/grbknddlj.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuzkoouh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvgpdilsv.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/ghadgbwcm.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuhulguq.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbwlgtov.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrpnayus.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/gtgloibba.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoskaylb.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/grelxsgqa.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgxeorxx.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjanfnwn.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gprvbmbzt.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgkqkhpr.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gwqozrztj.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/goxbuzwhi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrfajmut.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyacdwrzq.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvnljdyq.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/galssmagp.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/gukhsqadc.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbcxucxp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhubqygx.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gyiqxnitl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grglgvulk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghncibnou.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiwugvcp.sHtML


<!-- 参考信息 -->