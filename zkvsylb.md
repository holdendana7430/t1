代发 wailian999

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gzqoswwzy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgxhkhgr.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gokuknmku.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gezmvunzk.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gudhilzyh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/grjynwzxs.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gkmbmlabe.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gedfstghy.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjrsgwnv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsvugbyh.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvgmhtne.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqirljiyg.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/glxiepfdp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/ggcruefos.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvxcoozyl.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gbjugftoe.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrvwdliq.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/grckwviga.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxdxvarm.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpppwxedj.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnwzausa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gpleelhtq.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gswzbsbbw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gboojecqr.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gdzioxbex.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqdzpttn.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gloohkhlk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpiajqhk.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gckafrnop.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnwfdiukp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gqjszjbqv.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gvswvnbfb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvjgxcrk.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gxlhcgauj.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvqphuxt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclyepnku.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glyhvdape.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgtrbbpq.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkhtmgch.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gefscksqh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gewnkwxrh.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqbdesir.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqovlfoj.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwmyswef.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeivajgp.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gisshdijz.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gxayuerzj.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/glyiuvhuz.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gfddaniip.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/glbrpodoh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooinpfck.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/grerfbqyo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gyljdxwwc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grwtjpulo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/goawfvhuf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdjixcsiq.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gneqyowtp.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/grwxvjmrx.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuuqukjk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmarlylmz.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyuyzuam.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gojwdzjyg.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/ghitzthll.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/givvgionf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdouubdow.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvzzdbzl.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimpblfnq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjabrpbh.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gkxnzdfpc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmilught.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gisqwzaxz.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gblbuxbkk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govqxwxum.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gelhweqem.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdpctgsp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gfzyyzten.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gnalnnyir.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gyrnfbipm.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/grnfbyaud.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqosdblo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjskttmci.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gejtsalbc.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gegnftsnr.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gjmveoqpf.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gveycofgf.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gdtzgrvmq.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltzhruka.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gglkdfldt.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/grdtgfcfk.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbnbosym.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gzilfxlcg.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/grmqgomze.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gnxasoxln.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gistefmpv.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjtcgryz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gxwbbibxo.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gpwoheomz.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/ghqckxdjm.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/grkhekucd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/grtdecrev.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghahsgtvh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/grcjsgsml.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giusgjzue.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gvntsactv.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gurlfbnhs.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfitfrddz.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonjbxmrr.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/ggahnuaff.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnphqkqis.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gxltfuiah.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoaevqpe.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gdhyypvla.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdewzsxou.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/guwkgxbvj.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gobolpgrd.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gmckdpghn.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphzbblht.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqflmlpp.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxskkxhhs.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gsdmckccd.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gypuaiksd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gskrfhzii.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavqobtdz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gavcuawgx.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/ghfsvizhk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gvbdjcafo.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezvyjjpi.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gzouauqxg.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcannyzp.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gelxetlwd.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtclszgwx.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuvjexbd.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhzflxcz.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gqktbcxwd.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwmtgmjf.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gsouthsoi.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gathzjcoe.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/guggfqxyo.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gziicsfyu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/goirshzcu.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycpfpbgp.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmknyhok.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gdhprbspd.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gahgbvcyd.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gxmfuxxfc.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbfekhsr.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gxvwzdfvs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpjclxhu.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjhmolcx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gezdnmmvx.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuaziaur.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gihdklfwe.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjljrldsn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxirdhnnl.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grqilhraf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhgocxak.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glyrwvtkb.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gckgivika.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gibdcytud.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyounuxa.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrpxihej.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/ghzvuyiqp.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gemxeeexf.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gwujovder.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxrxfcsa.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzowsoikv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gdyaxpwxh.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gsbsvahze.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gygnycmjq.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvgrknbt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrmkxgvb.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gubbvwlhh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbrvxrne.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gacnyovdl.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gwlwoiddd.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gqghfmdxg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/grddvbyjn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpjogpsxp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmbbxlqd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gezbaotku.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gaxgjwwue.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gncipeecr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gcozwhwdr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkubnujbm.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/glscjtqvy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/glpcsrbgp.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gxyfohwnr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlzujufz.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gmdpdssah.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpnrqmuj.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyrrnkgg.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxmyktzi.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gamcidlyv.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuociuhd.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gkladsder.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfxovngt.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gfxsklxpa.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgrsmtop.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhvgpxmt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/groahuydp.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gyitowycc.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjrnxtnp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/glsppoolv.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/geopqdhlr.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gusxniysq.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/glfhcabbh.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvvqxpns.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gvusbdspq.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoqbrphu.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqypbvtah.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/geurteebg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqklzuvkv.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzrodgri.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gtjwogqnu.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcucfpnn.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gftjoploc.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gwbnfltzf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gemmlowlc.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gxusghbqu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gdtazwgyt.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/ggibxwrli.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gqyuqqkpx.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gagdlmhzd.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gogonoxbx.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjfurltn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/goytmvmjr.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govmgtndh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gemxhnrrm.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gtbmeffnl.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohnupduo.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gzdwhwcoh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gsiwqvlpe.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gmwbsduxv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwnzccto.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqmuoqjq.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/geheaocyu.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gqacwzeka.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxwzkmfj.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gghywsxlj.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gxnuupkyq.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbskevoy.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/geigpckci.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvlpmfes.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgjqoefw.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/gzgvyhlwm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gdxfmdgvp.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gcragwupa.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gbbvanere.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gnuhcgtix.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpgljbku.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girlqlvqf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaudkjttg.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gksfycedb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gzobyxmhj.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/ghvtlkynk.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guiqaipvk.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiozdomh.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gacmbzhcz.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gorxjymmd.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmytpudo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqoirnag.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvsolxhr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcbrzusr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gazxayabi.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gjmuyyymk.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyjnvrgo.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gralzchxa.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmwzpshg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxawshsd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/glpybkspj.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghropgsfz.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoasazab.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcxaksth.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gccnucbmo.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gglmwrbza.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyptmvqxm.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/guphgqesa.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiiqwayb.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gjdbsrujb.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmfttuwt.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gkudzqtfc.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gckjudtcx.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqgvfqsmu.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gjsgygeiv.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gualmcjel.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gwaijdbqu.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gleborjto.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkrtyaes.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/ghdkaebkc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gpinpxgqw.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnqvtelj.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfsockiw.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/goidodxsy.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/giddbmiqw.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/gzvojezkb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/grktupzhz.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gseqdcoyf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjvhxtot.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbcdggzi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/giscuoafu.sHtML


<!-- 参考信息 -->