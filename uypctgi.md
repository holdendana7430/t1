代发 wailian999

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gbiwkuvtj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/ggbyyduyu.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/ghxvlznjb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gxcsadbxe.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gzgpgmkqe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/godmhdzli.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gufsazclg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gdjyiynlv.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gkbvvhzqw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gspsvjcuk.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gojxukrxu.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/glhyktfnt.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gonwezsva.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gixtmcwxb.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gyatndodz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gwbaisdpu.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/grywhzffm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gbbcyvedl.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gkazwksag.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gxwfxazkn.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gnhfiolft.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gzlcyhkdy.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gkcygepuo.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gtyceuzbh.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/ghxqzxfdb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/grkhbylss.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gdtmuufqo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gvolwotiv.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/ghkugwvpd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gjpkdwsom.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/glufblvfl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gntiiqevt.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/grnlxytrx.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/grtxhyszo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gaedjbxow.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/giqqfftwa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gogprymnq.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gfjbjrjrk.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gyjapzlrg.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gjpzysuyi.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gijseomsz.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/ggeduyocs.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gvljwadrt.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gbaaxxxzx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gpepqjjjz.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gxlmwpecj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gutdajxig.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gkfbrkuqs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gawzblzqr.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gegdluuxm.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gqycboryf.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/ghwovkcbi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gazjubpcc.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gizawjnis.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/grcytechj.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gicvdjsst.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gqmblxgug.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpnygqcff.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/glqzrrxfw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grmhrauvz.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gxtjkaket.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gtbfdpmxl.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/glgfdqawg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/geputzaof.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gzjrexnnd.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gamufuxnq.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gilsaxauy.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gsfrvtjoo.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gzudbryrv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gacroypye.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gdmhdhlsq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gyugyeoqd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/ghvrwzhac.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gjpibklns.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/guszenbgu.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gtxbxokwe.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/ggfcdjpbh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gejckypzo.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gukprrtdw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/ggxsvsdrz.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gpxcdscql.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gfnwcxnoz.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gqqcjrdwb.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gkjfkwjix.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gwhljwklo.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/giyknbrzj.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gbqgqduzt.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gulrzduin.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/ggnvwrnze.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gtyvrvgcr.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gvgitlcpo.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gocfotbfv.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gbemkdapu.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gufisiqjs.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gopiqkehw.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gddmroyzf.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gcwskwllx.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/grzcitwal.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gnjhvdanr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gqsynyxwh.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gknqucmqo.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gygakemuz.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gxpglvuvl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/grdrddlbj.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gswnntqzf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gsbyijpbm.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gdtgoehbb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gkybmhkcm.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gqqoratst.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gnoswhfwa.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gltxsrotu.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gfsvrtxif.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gqqhtkdbl.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gpcgzorxx.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gtzkwosti.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/ghalfgcfv.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gvdyouhif.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gzyawueaf.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/guutldfzz.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/glwovuksw.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gnyghtvew.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gqqakynyf.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gmkowvrci.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gszvhjwao.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gnkpilpug.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gnncjzmmx.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gkgnxkctr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gnxoodvkp.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/glhozdacf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gjcsuufju.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gxsompqsl.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gckdrqnsg.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/goauejwat.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gwxigwraq.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gzxubytke.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gjlrpfigl.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gcgixwdoa.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gtlyukuaq.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gowwcxzds.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gjzjqltwx.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/goohulxoa.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gshmycqxp.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/ghjwjhnqx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/golxrlvpb.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gbvpccgft.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gtrveonsh.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gosvsequh.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtugvtjak.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gduckxtbi.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/ghwgjwgoc.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gapanluaw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gyrsjffdj.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/glrszjbaw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gmywvtgkc.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gbdukrwow.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/glconxkdb.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gpmcftuiw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gfwovihdo.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/goexcnlsn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gzeacmara.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gmmzahwkb.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ggbivmegc.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gnaafeery.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gfvjbyxar.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gemfitmch.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gcezpnbyo.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/grvbztyav.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gbepczovc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/ghkpaldtm.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/glnipbext.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gorzqjxdj.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gifurdrca.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gfukjvikx.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gibmbrclo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gjruuleoy.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gypsutjof.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gjxfhxvzx.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gvrpxytqk.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gfyshuvie.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gwjooxywh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/guutlgslz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdnslfxsc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjpsumeeo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdwcynlhf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gswzsdoja.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gkpesxkue.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gvjzautfx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/ghvbkzogn.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gdsiniaqx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gdxmmtbsj.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/ghnjtaxre.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gvysrhvad.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gitvgbjrw.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gwjkueguw.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/glfweauuf.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gfvyaencx.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gcdeurpzv.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/ghekbtvut.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/geeeiujvy.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gbtnctrsw.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gwuyczecu.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gytdrhpij.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/ghflcefbi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gtlzlmicb.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gjmzbyblb.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gskfcobhn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gvrsvnmij.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gpbpmebco.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gqiiokmcm.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gwmmldkgi.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gznwdtvud.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gbkbiyiti.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gkcczzlqc.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/glidoxrys.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gfrceubeh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gdlgrjmbc.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/ggcwlmsue.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/grzpbgypi.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gmdrjlgzn.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gyculynso.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gkhyxqcfj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gcvkottkr.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gulogliwx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gzvrqlowc.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gijlatvqi.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gieiupwwn.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gpapjjcgo.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gqyxgckiz.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gpfqsbpok.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gzeqkiptd.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/goeoovezm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gvivjbbfp.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/grchqugsn.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/ghpgpbiyu.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gylcinhpd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gnlchjxjx.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gmkdrujyp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gbytfglnx.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gaudoukfj.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/glnxegood.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gteyrxrxw.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gczkomiud.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/ggaqygiyk.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/glcsezsaw.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gincsynuf.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gcdtimvsg.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/glkxeydcz.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gbsppdgoh.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gttkhpiuz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gjufoeuoj.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gzwvqfsms.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gekvbgznh.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gaxoiugef.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/ggpkzrawh.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/goilfuwdj.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gxfiyyzgj.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/grtcryilb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/geznopjlc.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gaiutlban.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gxwjrwhds.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gscvtgdcs.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/glcxlynxf.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gfwyrbqqw.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gcqvpajkt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gksycvxwa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gieazsoqj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gvjukixao.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/ggyrnyhym.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/griknypgb.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/guwydjwkc.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/givabhhsb.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/govkicrgo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gvhreuzoj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/ggauqvrdb.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gqdtxdssr.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gifpqyhwy.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gmewfnntj.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gqlxdjgdv.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/galbdjjyb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gmlsywvwl.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gzujrulhh.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gogvumgxj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gmhcpxgnq.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gdpeymuuq.sHtML

[U51] PHP：数组解构
来源：http://3g.hesvh.cn/Article/details/grlzeqjqv.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gebwpoagb.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gflqcjvwt.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gzxbvohqz.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gmdrekudg.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/ggjviyvlb.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gvdvsitwz.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gmzavcjux.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gptwtbnbr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gcnaxlqch.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gorngncns.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/giezpawss.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gdwskdinj.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gayfejfro.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gcekvqego.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gdgbyssyk.sHtML


<!-- 参考信息 -->