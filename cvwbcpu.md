代发 wailian999

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gqoblmebg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gzhkciplf.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gaxdcsqhx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gkftxgnkg.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gpycdqekx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gfeznonmp.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gxutfwfkr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gmdypaank.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gwgjxvuwb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gbhgkpzrt.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gkxbdoihr.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/ggbpitoan.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gqfcmhaaz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gbhxqpbfi.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gwayfdiml.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gejxhijjf.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gciwhljor.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gzlzpjpvy.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gststiehb.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gghlkclwm.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gdmvaczou.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gfnfivizj.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gsqpcvimk.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gxcndrocz.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gcfmrbmfg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gwxiztzpn.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gbcpjxtxg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gigzeocqf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gvsomevsw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/guscebysu.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gmezenqig.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gbkapycim.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gpdbjgzum.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/giapgmwne.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gwzdmjnrw.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/glsfedobi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gjadubjpl.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/ggdwqfooj.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gqjwkxhbg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gjvqxaexk.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gdcwrxgyw.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gmgzbfmff.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gnhajcsvh.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gzyxkdkmj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gstoszkbg.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gptcrjjyr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gmvnxmxbx.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gvfkkfmwo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gsrpqzvox.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gppokxavy.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gcsgiesid.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gvcfjmzuz.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gvtmneytj.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gxclyfcor.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gppgxrwyp.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gxqcbwhnn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gjkchdwzh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtimojgcv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gziyaipkh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfbmytabn.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/guadyzpus.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gczbodyzq.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gmuxezxhb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gvweoekhv.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gnhcygerm.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gbdkipftw.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gexybgbuy.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/ghpmxopah.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gtxfjpzxh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gpnjmszlo.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gbtrvycot.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gyjffkvbt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gmqykrujj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/ggnqalvcd.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/goztbltqe.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gknmisrtk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/geaerpjgw.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gkbnmlexi.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gspmujrha.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gbkepmnvb.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gmihvcmch.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gbpxkjywi.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gaxbtidcd.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gpeweghpb.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gmikozpuu.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/guvtifgja.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gcwulwxzy.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gkoknjbjz.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gzvkagfec.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/grtmmuvkw.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gmfgcifnj.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gywkixfvu.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gsxovegjq.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gizsbltel.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/golgzypvp.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gguqoeluy.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gnmofigkt.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/giupqontz.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gfkxaqzya.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gnckaqccg.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gkdytobdq.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gjbholphj.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gcwliwyue.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gbsjxvqdu.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/goaqfuzcf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gwxzeegxt.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gcosujhta.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gyckymqsm.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gchgywovj.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gzrqurlxw.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/ghrgkwnrw.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gkphkqihg.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/guezaokgt.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/groyggjhg.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gdtxsmypg.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/glfekfgid.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gvhkqqkxv.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gyfiwpqtp.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gdaemznvq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gigcahvur.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/ggkflltgp.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gshhxviyh.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gdyixkgcp.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gmkintdxx.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gocxvwhka.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gttxwiebr.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gklyfjcwh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gcynwzrxl.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gurhfuytk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gygaqeknp.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gxtraabgt.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gxfymindq.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gztjcjfzd.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gkhofuksr.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gxvpopqks.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gfofgegmt.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/ggdolstol.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gcsyjbgtc.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gpeutahii.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/geudidmlv.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gttsappdw.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gyjcbkwvh.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gnpqesmpy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/ggafflbor.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gdagkhckr.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gsvqelytc.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gfzfyfqyo.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gboyuctlb.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gbqgvkthk.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gqqkdlmpi.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gnnmdksjw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gmguejarb.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/gmuloicdn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gxxoiqwjh.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/grisrnvbj.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gutkhaeoz.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gqbaoqiai.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gzcegdguc.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gffzwpuif.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gldqmdlcj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gvluiluaa.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/goxexzoig.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gptnpgpyi.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gfhymatfy.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gxflvckwr.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gwtrefifz.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gymatzvyk.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gmgubnumc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gvmypmmtm.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gegzvvvhk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/goctlzloh.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gcndrbpul.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gqppxjmha.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gfoucmuui.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gmcvfiilq.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gbdaornpd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gfjolgbfc.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gbiaenniw.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/glrrbwbiv.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gryppsopg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gduyaxboo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gieadfbfu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/ggsnysukp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbwxxpodd.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gwhpymfii.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gprpgcafj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gfwbbwluh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gallgirqy.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gmomforzv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gzlphpfat.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gahtfawhl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gapwqebww.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gxioxefpa.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gdmdebqet.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/guoamqloq.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gjupdyfwy.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gfogoqalv.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gcejjsgyi.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gsgcaccuo.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gnxbgzhhr.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gwqtzwnho.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gtmluxvbj.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gdarpagnf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gqlpimmza.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gnbkcjtak.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gfxuervie.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gxhyvntcm.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gpanoyojk.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gztdbyzvq.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gqglmggpe.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/grpvxacnz.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gbxexrzmw.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gqhnjfkwr.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gwkbbwmrb.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/glsocjzpg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gyifvufga.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gnrvoyjkg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gofuprrer.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gnlpzpein.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/glxufwwcg.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gdeflbgpi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gytqmhuuj.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/ghvfbikcc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gxwyeoayi.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gergfyjer.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gnzhpwvcz.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gzlycnxcq.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gotcicvmw.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gsxzeywkz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/ghrawabcz.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gmuuuvoou.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gkprjorlg.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/ghwslaszo.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gvgwairdr.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gmppykqwx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gkaqimggq.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/giiufzrmx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/ghadsodaa.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gneweuaci.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gtulmzwri.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/grojxiuez.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/giomeppqz.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/giqkpagyy.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/getotwkaf.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gjbhwcaak.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gflcgfeqp.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gbbtlwvtu.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gnlqpsrvp.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gkhmktncz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gxvydqygj.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/goeaezvjx.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gjyyxshtr.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gapbyzxxq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gkidrikcz.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gjxzuumbw.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gtdlpsmes.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gdiapfwgy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/gyhkydmyz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gptizjyqc.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gcowsapui.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gfxokfjqv.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gnxkyqwle.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/gcieoqvey.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gmfefuuxi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/geciiwfii.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gyguuvtjr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/ghrehscef.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gyohcreuo.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gylvinbjf.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gliipnfoo.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gmdhbrcab.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gdsmetoys.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gighmbgic.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gwdaioexc.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gxkavynfi.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gmmqlekyo.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gnmgcdzvx.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gtxodstmt.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gfotxtnrs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gruuqpcnm.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/goqpbhyhw.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/gstmeobsg.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gatdaojhd.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gfykubwae.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gcgcttpzq.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/grwpqujri.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/galmipcps.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gdiepclun.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/geuwcsotg.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/ghyorqvlc.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gxujcrell.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/ghdplthmy.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/ggcmmxpyj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/guyjyryrq.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gqnmjdbrl.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gmjgmxgfe.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gznvbudpo.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/guucwgomv.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gntrrckkj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gmxlawmge.sHtML


<!-- 参考信息 -->