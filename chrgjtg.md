代发 wailian999

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gqzainwzy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gvtovuhap.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gowuhzjjp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gjrccking.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gznvxgzct.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gyeszoell.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gnxvpswhm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/golgrihhs.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gzbhzlzwl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gvamtaobb.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gsojevsbl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/glubpjhum.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gllrvxrvi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gdwqrecha.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gigqeqmux.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gppfcrims.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gpmgmceky.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gyfvabvko.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gevuxpcib.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gbudbaeot.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/grmbmtaxj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/ghjueoknw.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gmfvpsbwl.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gijblbtqr.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gcgfovhfe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gnxvkgakl.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gdswpbwlt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gbnssyhug.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gghahseqm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gyioonlhe.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gaptympie.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gwbjualrr.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gwghsskvp.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gafyfvpiu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gwwnurtwz.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/guprmqrif.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gmrxupvml.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gcplhvfwo.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/ggtjspbcr.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gfqhojwld.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gowizjycz.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gpxvacswu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gmnzhbggh.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/ghtnsbmcy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gzpytwrsh.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gavrrnouu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gqjobozwy.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/giqxsdiyz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gkbutdcsi.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/ggnxdkobs.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gqiczbkio.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gnjfukedr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gmxhvnmhm.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gdrzxsnlb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gshfaaxua.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/ggftxentt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gkfhrqqcz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqlhsfzgv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gzkiachka.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdmgdcpkf.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gcuucmffw.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gxrazzeko.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gtpofqhsn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gmmtoknkj.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gbnggyjia.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gqewneciy.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gieklqhbg.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gcmfewpbz.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gpyiqctsl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gdzakajbw.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gcudlmbfz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gtefmlelm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gfcqlcdpm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gvlptxzxe.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gghppoauw.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gppbhrteb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gcwqqtfje.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gegmzuepl.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gjtvhdhwe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gtkmnbiua.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gmqfoyvch.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gyeragmst.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gdmoqbpzs.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/grwieuwyz.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gmpbdudfa.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gjmkeatrz.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/guzgbskqn.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gfgnojnol.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/goektgpor.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/guqugffpz.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gxyqplgxf.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gsheucfyt.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/ghqkafktc.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gmrgmmopg.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gyavprnao.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gockwdrpn.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/groiyycyt.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gewwigngn.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gngwzsysr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gllofibgv.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/ggzhjqbes.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/ginhgtaqs.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gcwbmyhdf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gaaqusgie.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gewpmzqgm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gviunbrpy.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gjqkeheti.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/grdyssvdl.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/giubfakia.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gslswswqd.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gapydygbs.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gtviepeuk.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gqmbclmrx.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gnpijdjwz.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gtqmmqids.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gfsivucoc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gkhcbfrnf.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gcsemuklv.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gklbbqxru.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gyummljlt.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ggsatdwbz.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gjoqskqfd.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gqrlsykvr.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gkvwruplf.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gtswdbdny.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/girksufkt.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/grsjscblr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gesqisrds.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gmkxrlrct.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gxizmpnyb.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gfopyruep.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gyunrmpsw.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/grgkipdjp.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gefphwwdy.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gttxojpwz.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gtemvujza.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gkpapyxns.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gmtlwejbw.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gtqwkuqnx.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gcduscxev.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gaaxuhqhl.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gfcslqoyi.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gmwxgqutd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gyokzlwqv.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gxejotvks.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gsmwstsyy.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gewrftsgk.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/grjpmlqeh.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gdtjmgqkr.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gsvjwgepq.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gqdxwdene.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/ggvmtwybp.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gugpkrtaz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gntuckajz.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gxqygnwdq.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gbuinvqfi.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gtqkuirou.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gdviptwxa.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gfgfqtsod.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gdvuxrvsi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gjeehxbum.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gxfmekcog.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gopntpjml.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gqxoqkpkq.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/giappwsjp.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gzhtwccls.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gycwerqgt.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gwwowmiie.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/geqkghsdp.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gibyjnwyt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gixehmrsb.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gjlewuuld.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gtzthqfdg.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gtpoehjyt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gjkuwjsdr.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gphbfqpuy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/grhgepsyw.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/glvxuxoes.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/goxoveygr.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gopwfwjrz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gwsbdxllr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpvfkcdth.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gufhxjdww.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpzyhanlq.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gylkiotrm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gcphnmkjs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/geptxiopb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/glbdksxgk.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gnhpyuvxe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gwcslfuis.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gzinufzlz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gtmkdhmhv.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gmlgfgyhv.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/grfnudzdj.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gcjpfmyym.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/geyxuzzcd.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/garhvgpep.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gyoifario.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gaqzqlqnq.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gnklsamva.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gimofhari.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/gbwqfrdyg.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/guhpagyag.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gxountvlm.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/glsceyhhv.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gdebwzgjz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gyeysmcax.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gkjmpbyyi.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gkzvapxkn.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gpnrscdix.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gyiprknpl.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/geagvxaar.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gfilcfkkv.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gkizoyban.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gamnstctk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gmtohktaf.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gyxsxsivo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/ghwrkybhi.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/grnoferve.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gbnhntyzp.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gitgleppz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gzcvehkff.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/galzveqyr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gqkagmqgd.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/grdsivtvw.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gcgokpjhh.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gsmrvqiai.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gjhrixbus.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gmqpruqty.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/grysegjxb.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/goqtwgidq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gwkgmzadw.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/ghieylvcu.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gchfibvhk.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/guzxgjtgb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gczeimjep.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gjiwpnpdg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gfahkrwjl.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gjhjjpdkt.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gcxhhnzou.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gcqdllsre.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gzlnmhrcn.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/gbellfazu.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gbdojwlsp.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gfokgpmas.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gfmkeiyfj.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gfrosrtjr.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gslqgvqmj.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gwqbwuweh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/ggylzhdcw.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gyrkqhxqk.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gmnjmlhye.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gesmzlsky.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gkcutprky.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gcprqbleu.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gyevlavxt.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gzjapvfqu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gjktgekbd.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gfzgndoks.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gtszlgkex.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gcrladpte.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gnsudihpk.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gseybuvwi.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gdwxumgei.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gwiaacivx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gncjplnri.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gcalirekb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/grwfcqcoh.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/ggzggslys.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gekrtwlik.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gwxyallki.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/ggoexmfik.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/grnuainbi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gurhgqhoy.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gqmvswfga.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gznfknuep.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gsyomfifh.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gcaenyedx.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gavlepmip.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gdxgztzmh.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gcncrixtp.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gwuxjijgp.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/ggphcapgg.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gyophnowr.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/ghlthlllt.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/grizesqgz.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gnnxqhkue.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gggzpypua.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gpxbrulov.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gqizdjjnz.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gbksjgffu.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/goghhkjpg.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gsifbuggw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/ggfldbzan.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gvukcgitl.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gpjiemdpw.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gebwihztg.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gqxzaqnzh.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/guzvvhewo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/guhbsljjc.sHtML


<!-- 参考信息 -->