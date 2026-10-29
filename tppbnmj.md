代发 wailian999

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gqvcuppxy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/goxpiqqhp.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gvnlorihl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/ghjcdgvay.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gfmynknqi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/goqpenyqx.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gleeemuhl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/ggstqrmzj.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/ghzhrvivd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gbjqxosvz.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/ghcogvpat.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gpsmlyion.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/glebrbrto.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/grmlydbdq.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/ghoylsjbc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gttkzakfj.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gslupqogj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gxlxgwueu.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gvrdsavxp.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/guilbxvig.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gayovdtor.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gzjgxhubz.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gunspokvg.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gcvwnxcwf.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gairriwnr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gmiqnvzbi.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/glwiltvqk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gaewikptq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gbxmanepz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gzdppenbu.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gggvnzmlh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gyvegkjwt.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gkcfsxhov.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gutxognbt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gpclxyyie.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gpnqfrrlu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gqkvpzrif.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gjwfqwbjz.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/guomxwtse.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gzwxdseqn.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gzvswkxok.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gxyvjbonp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/guqvuxhgy.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/ggoitzmsm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gcqwipews.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gfhsbtvzk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gdnhqcwss.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gampuqxsy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gyeehpgdj.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gopxcffst.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gnmrhcbji.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/ggrcvamjq.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gvfbdsiku.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gwgjvhoix.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gzjjuocaw.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gonpevadf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gpvvkhqgu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkwqkwhjh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gcpbzqxmu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grjzjnnik.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ggibcrxlf.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gkgwcbivo.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gxgznbqnp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gyqsknurh.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/grspjniol.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/glqwssbpt.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gbdkmjktk.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gxwddxajf.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gbwyegzfy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gapvazxae.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/ggohowgdx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gkzeyecqq.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gniteikze.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gimodthpx.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/grvzkcazh.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gmzfthywu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gjwejqbsv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gxzvngbjs.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gtxljbuzo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gmhguuqwf.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gkbdgywnl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gqzrmixiu.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gsjfuwtqg.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gxqctevqh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gdmcojeao.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gxbdcgjle.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gengpjlwv.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gdsficocf.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gmdyibyiq.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gelvdyecn.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gafsmlabq.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gwlagzthc.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/grqbeihod.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gvfzdlvom.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gflydulsd.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gaosdvxdt.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/glyzwuwmo.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/guorpthjs.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gxafajgna.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/ghqgluspz.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gsxudxdqj.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gvcnklenk.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gutsazbmw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gesedrhzt.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gylkpfeac.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gqllmwpso.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gytckhjxx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gctvkokyu.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gdbqhdzoe.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/guhevimtd.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/geiapcjit.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/glyzkppxi.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gnmjvfbpm.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gjgfftflr.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gylhnqqob.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gotdlcqal.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gekhmcozx.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gwavxppml.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gkriucxwt.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gibyekunq.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gsglundey.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gilzbodts.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/grulkhhjf.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gbqduzyqy.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gicfzbrac.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gyzcdjrln.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gwilrnvxk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gemlgekpc.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gbtjdkghm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gwyijlvcn.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gmqzqznkm.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gkaktszgg.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gaunuzmqg.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gefzttbwq.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gtkxauqux.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gqmlsjuio.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gvljkfxfe.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gjdmaoedp.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gmfwwwiik.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/geouchwln.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ghryoqbyd.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/ggbmvadjh.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gbjsmuouo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gwpswulkp.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gwxezqoda.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gygggydwy.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gtidjlfpu.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/ggityahzl.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gxeneffqi.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gvyvdtjjc.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/ghwbwjzfa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gymedeosr.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/galvpixax.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gyzlxinwx.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gmbubkmum.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gyamhxboz.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gwwayfsth.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gpgntsfuz.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/giaoakcmo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gmtyahlmo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gvallptrk.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gqsqhbuae.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gfbtfetrw.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gzjdgasyy.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gwgcqauzn.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/ginyqtkhq.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gnvdyqhmr.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gvxzeylqu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gagvfnght.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gokozatna.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gfttoesii.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gixcdbzye.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/galepobmh.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/grkwgdnzb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gpiteyfam.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/giqkigyuf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gkjlbqxkn.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gwbzqzfyt.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gqocdynxs.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/guhkzdzvi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/giutfimvq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grwtrcdrk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gjziylbes.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtlbxtmuq.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gmmflnpbd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gwesxijve.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/gjkrjqtaq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gdbpnqysq.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/grdnximpv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gcypoaxcr.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gvgtuzzje.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/goahrvmth.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gepzowrsu.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gkfzsldnl.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gdjfxzrls.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gykbjyuqd.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gcrxqjsnw.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gmabdrnht.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/grjldkqml.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gcarlqavt.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gzjhcscvg.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gokqhuzun.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gzapfuxtb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gpvdrmdmj.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gjdfikfmf.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfjrzqoki.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gxovqmfbh.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/groovgayr.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gqfjawsfc.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/ghsaogngw.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gtxudpxfk.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gzjckqlwn.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/ghkbqtpss.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/guyemwguq.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/goriudlth.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gwkobrsyf.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gwskhqgbj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gugmzrexb.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gtqpbyxnm.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gqmzyolcl.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gdxglnpdu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gemzfhspl.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/glqnnxtgw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gukuiqdib.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gmqilkiup.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gyrwvhldu.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/giphtryxc.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/ggeyrgmwy.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gvtxhwbah.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gengnzrfm.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/getutgoua.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/ghxkhwwcn.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gtdtnhfcl.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gnftyubhv.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gaocednil.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gewucgeey.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gqaaqbtzc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/glbaoxyku.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/ghjddhlmz.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gvfcdbuzb.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gafswdcec.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/gjkibwajd.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/ggizvzycm.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gtwrsbqjd.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gdeosgavp.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gpdchgcvr.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gptddsetj.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gyehsexrl.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/gjafnscei.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/grzvbejyh.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/girafsgkq.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gisrltdud.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gtfzcnrtt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gqnsfappi.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gelxrowmt.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gxxtvxobi.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gzonadglc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gylqlxsiq.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/ghjraffwh.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/ggdidpnxn.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gjupyroxg.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gboqzsabq.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gflonkyhb.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gygvwelsx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gfkusqvlq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gtkhmdlvn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gshhpezmp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gujjxnmdk.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gnjgkqslv.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/ghvjxveyn.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gyfserakr.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gsplriztt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/guscvigia.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gjanarlby.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gioorsdbo.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gmlglwook.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gdlhsznps.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gheywzamd.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gfuzrbozx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gpfvvcxwa.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/grtcavfrd.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gvatdtusi.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gqozywmvw.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gufgbmkow.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gzqcnxhnj.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gtsdmnkkr.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/glpdtbnse.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gagxbdfbu.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gjomojbxr.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gwrqhtdsv.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/gynrilpxh.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gdoyrexjl.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/griorunxd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gkuhopgbi.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gyzhciwer.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/ggqtuqetq.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gbvelyttu.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gxmtlqrcy.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gtkvyzibg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gjduyudnu.sHtML


<!-- 参考信息 -->