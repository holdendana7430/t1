代发 wailian999

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gseuaakme.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/goblminux.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gfzxchhwj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gpeyebkny.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gvoifawfh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gjzkfmtwb.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/ggirrttjq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gzwdvqkpi.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gefqagwdc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gffesxsqw.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gkwfsneei.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gvfvotmag.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/geirxlyjf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gilvciybu.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gptkptlnr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gudvjukcp.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gdsmwkilv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gizpbqgkg.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gkbomqhkh.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/ggunuhbpn.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gmcblwodf.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gmomcllmh.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gfgyjqrwx.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gqulcdvth.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gxbanmezg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gqufxeumw.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/geycdfxbb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gqmtzygsg.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gypyxujne.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gjtueuvwp.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/ghijbzrax.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gmyfytcrp.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gguqzgoek.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gtcdflljc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gkxlowhnu.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/glxiutqcr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/geoizbcxf.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gcirswofl.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gaoahsuty.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gcgfftaqo.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gegjixlrd.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/ggrbiitax.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/ggxkclqsg.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gugmaaasm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gbhrbddaw.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gwodhvkmf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gkbkbcxqn.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gzffnyivz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gnygoyops.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gptpjpkrq.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/ghinlikzg.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gzfikuxje.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/giclxyijd.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gvoucdcko.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gziyhygxm.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gwxuvuflj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gzofvygff.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/goggkapjh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/goplgvkrr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfxbpflil.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gwdkcsayf.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gakxxuvtb.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gxoffxuho.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gauadliew.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gturaaxbj.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/germuifzx.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gjxvujegp.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/glsdipdfm.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/goitkgyph.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gftlcxizr.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/ghyjwxyvn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxwvigljv.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gzhlizsay.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gvlzuuxxh.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gljlnezuw.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gkeleehzm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gkdcmjrpg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gzpxmtlis.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/goaaavbxt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gufaxezpk.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gjfyvpygt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gcyddhnof.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gjwmfxebk.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gwccnzzlf.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gadwzslfv.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/glkzlghew.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gguepjfbp.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gwzabshov.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gclqgacer.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gbgqmrsuo.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gnjpzkuqe.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gilaabcrq.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gylxerxkm.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/ggsurvawp.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/guqbrvwts.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/ghvurkejf.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/giuflwlzv.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gxvkmbgma.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gvszkkgof.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gffmohdsg.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gbyyhbrma.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gdqrdbvhg.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gsiuqeobj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gjyitcwzn.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/glnmnksbt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gchaibcwe.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gkjbyrffa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gfqklfcfb.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gqiyyawwe.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gjkkvvpix.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/guqeetbtj.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gnolihuul.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/grrprkqtn.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/guuuwejvl.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/glidzcepa.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gmqycpgjz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gdkvpzggq.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gkiavuvdw.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gpnidyppr.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gbgtfglnk.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gaejznumu.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gheaggjtm.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gvysjymvr.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gzdsgmjer.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gdqqznuco.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/guxagyqaf.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gmyefcvbi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gtvnrydfq.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gllzwgmnt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gartvskzd.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gwffqnswq.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gxqfijcfi.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/glgwvphzp.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gkevwnyfs.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gurbdabim.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/godibsmwx.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gerfwwlnv.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gnbgtuyve.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/goadnzlyj.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gslyfgwmz.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gbzhjylzk.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gsjdvelqm.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gridpscgh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gyucxqrua.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gqbxkwppv.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gqyeyjelc.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/giiinhkjs.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gzgcjlilc.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gtknpydru.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gljpcofby.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gwycgofkb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gidmtfkyc.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gowyswkio.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gesmaazur.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gcwxowbbq.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gsyozlobm.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gpinmhekw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gfbchkpfp.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gateclmyd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gtqeznekt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/ggnvsfjrj.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gysernyhn.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/ggmtwpfvi.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/ggrjijhnr.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/grkbueijb.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/grqtcqqqh.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gjchomytm.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gkdpacrsz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gnwmvokkf.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gigpjpapr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/glhztcqef.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gppaoxkmt.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gdtxovuyb.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gafnwytzl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gxrlunmyd.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/ghwmgngyw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/gmhjcukfv.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/ggaygyalz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gztdbaoct.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gjlkmypnx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gvssivfyo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnsouzver.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gsjrkdszs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gamyciiqn.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gvxyqxnxf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gkrwymbjo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gchbygrep.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gxlteiqgz.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gwddeztrc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gzedgvduf.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gbwnnfjjv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gqaeyjzxk.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/ggyxtlfjo.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/guyhiygec.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gpecvabog.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/giyqiblaj.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gydlaazrj.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gasebtywh.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gthbnkkdh.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gabgcgojc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gdyhjhpin.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gdnuambkh.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/ghiejrohq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/ggktsuipl.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gnmjolorc.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvlzjlrlm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gtzxazdoo.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/guxxlmbsm.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gmfezpqkv.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gmonvvxox.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gswnlmbwr.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gzlxbemvc.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gvgxabxyt.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gibpiarph.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gagumpknf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gexotkcyu.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gslyqvnkw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/goeposlls.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gwiwnjrjz.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/ggnijypiv.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/grtttjvqw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gngucoxxw.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gzmwbgtdn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gkvnekifk.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gpkwizmnw.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gpdihjqcf.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gjktnmory.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gxdinjqfv.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gnjkppsmt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/geftyhhxr.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gugtwdlkw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/glkjbxwva.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/glgxkgysi.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gqqxuaftg.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gnwfwlrwe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gsartzqnf.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gcbhizaxe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/ggcmhoujx.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gfzcqqzgs.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gknhiqgif.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gqbhznghc.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gyrtvoyed.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gtneipjoe.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gcajjjsnh.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/glghcjhgh.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gxxxvxxev.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gmersfxgz.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/glcytkthv.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gtambdhkp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gbsqcyrsx.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gdzwylzoc.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gfvlyeaow.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gqvbngqve.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/glqiwykrg.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gexzbavke.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gapcdvjeq.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/grextgmzd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gvyoxubpe.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gxsyvslva.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gofctixic.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gzbtbdobc.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gjaublffz.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/ghzkydrtc.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gbjnnalze.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/ghqgfocie.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gdycpmulx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gicvhtwvs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gsqianbow.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gfsllfhfo.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/guyspwuio.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gfpwahtmq.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gmdbygniz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gpcwktlzd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gqheprije.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gclqjaerr.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gudzefcrk.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/glemlcjnc.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gjqhufbuw.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gmlcliyps.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gnxdjaamk.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gukxiksfd.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/goehenffu.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/gfaabtqyc.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqunwlcpo.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gnjuvqxtj.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gaecneagw.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gzfzvsbry.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/ghiiuxadt.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gywevpjys.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gochgbfwx.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gkegepwar.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gpgttcdzv.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gttylyeok.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gnbrjxbeu.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gbvekieca.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gfmpzamqo.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/gvvlshzmg.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gkpsnyipz.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/ggvnexsze.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gbywnfubg.sHtML


<!-- 参考信息 -->