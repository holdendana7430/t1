代发 wailian999

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gsfmltdqi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gbxqsyqef.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/glqqvqjmx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gijaoenkq.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/ghuxlpuvl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gfzqkzihu.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gjklgwlga.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gxxzdfucz.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gnvqtjatq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/grfcpxmze.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gppxdlppg.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gsgdnoysk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gttsojkpn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gdbdzurxb.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gxfcoqceg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/grmvgqbjk.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gxlsfeogl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/geqkqbftx.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gqsfrpjnz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gczcairqw.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/glmaytjkm.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gdprycvjs.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gjexzejhp.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gxxxbruup.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gugumqdai.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gxbknopfi.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gvglkqjpi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/ggxstbgkx.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gohltrndk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gpdnghkas.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gomhpdysr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gvggbkzuq.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gesaxtxwr.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gmszgsdbt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/grozsfhsh.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gwbsgojbt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gpsbqyvox.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gtgodmclo.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gdbgapgye.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gimdtmaid.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gbgedbwkh.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gxxtwhzrx.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gqjwqqmrs.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gokkydqec.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gggggscgh.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gpjwkxrhs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gakrtphwo.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gbnkibejw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gzlcqobcd.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gpoacnqzf.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gnlnnaymj.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gaowwgjtv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gdbodkgnn.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gtozpzjbv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/glevegoqu.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/grortdfky.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gworjfgpq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkpafdttx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gwxbljuwn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdkplmvxz.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gbaibrghu.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gwktjdlyd.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gcscbfuxd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/grxcbigli.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/geoszitjp.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gxpelluis.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gbwkkjkah.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gswxdiutg.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gwqbqdyor.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gkhwaoplr.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/googziwvw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/glyylyewq.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gzwyoftwc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxijrhtky.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/goyyoajfi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gkuhkjfid.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/grobdhbvo.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gpphnjlqb.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gbvhfcmwx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/ggsxjpvlk.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gorwbnhvi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/grtqepeja.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/ggabkvyjn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gzhahpbfv.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gbmxguezt.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gtkwabnui.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/ggqeovrcd.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gsczqubjx.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gnymzqbgb.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/ghcqweufz.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/giaqkqhsb.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gdnrgsgxz.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gmfcrrdyy.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gzkppbklg.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gssjoaiwd.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gheljpsop.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gioeunuql.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/guknwakgd.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gjijrzpts.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnoiwtids.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gexlogcfx.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/ggpqadulz.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gkdtcfhsh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/ghpngrfrc.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gpsfgkbru.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gimotcqya.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gdfcbwwhr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gvxabfcjk.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gwkcgbtmo.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gkptywsmg.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gkiblznwx.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/giudizjlu.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gwqvoaops.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gybihpfat.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gzuthhvte.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gwiwapebt.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/goqizmiit.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gwtgnzxoo.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gbywsukza.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gvdcunryx.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gyzyurroj.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gnpkhfeob.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gdjuqgeuj.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gvxlaytlv.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gdnslizia.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gdorxqkcn.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gixymshxo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/glfnbukrz.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gzaoesthu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gvchrbvck.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gaepyfgbx.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/glotmcrsm.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gtdtuxgpb.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/guaintosm.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gudvqdjxg.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gajovikys.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gcltcjnrs.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gtodjzevh.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gvgqmorml.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/grfmshwzd.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gogtwkpda.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gouoqopvv.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/grjiopxeh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gmuznnzzm.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gybgfasbz.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gkmyyioqm.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gfsztuawf.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gpjxrvghb.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gywxqtqpu.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gwfukgoze.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/ghptzkntn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gvtihlvoy.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gxnggfiuw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gmpqzckmf.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gpsuqkkwn.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gumuihdpb.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gitbyzzxz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gofengcwm.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gqsevbbmi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gnnbaqrei.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gnvjafgtf.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gcebniksd.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gmfdeuilb.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/genyistde.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gxhqzkqag.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gtinpogbm.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/glsktpswa.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gaglshwsy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghlyrogvx.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/glxgbdoqa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/glozioljt.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/ggmzzadca.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gwkzkllpc.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gykkdrgge.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gwgxhnyjt.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gejdyqmvh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gckajantx.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gboxcrhot.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gqmqrpukg.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gyyubkmkz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/ggsnhudwl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfjvpzyie.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/ghstgxhvw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glbunzljr.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gttbqadgg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gjowhcixh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/glyhqnkez.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gevvbckdt.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gqzfjbivk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/givvsayob.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gliygtljs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gyjendiaq.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/giqzqpule.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gdvwlvekb.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gykjezxpr.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gvkqfitps.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/grdquulzi.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gtqxilprz.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/grdkewwse.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gtrcpnbsb.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gyoqppufg.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gfizxzsro.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/ghatvhjbc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/grektrefl.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gvmnxdnrc.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gtbqadkiq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gzpisywvc.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/ghgnvvjjr.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gcqxlcdrn.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gfdizrkjk.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gaeurdxzh.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/ghnpursvj.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gnofqkwjf.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/goepjxezb.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gwidbgmqd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gsjqngako.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gyhavyevb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gezgrknil.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gevcxujfw.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gcfrlyvbq.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gqokcmgfc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gfyafnezt.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gzxhwhaqn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gslbkyqpo.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gnphfedrj.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gsshkpxgr.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/ghzwdaswx.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gvwqnlmyx.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gtcslsvxq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gxfyhthaw.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/giwqfnynx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gotvoqpmn.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gfjiockhp.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gdulnhtea.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gtjdgoerd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gnmeqqvbf.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/grwdjmsus.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gnglbmavo.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gnlxgevwf.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gfeyibwrr.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gzfdqcdji.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gkdtcvhnb.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gavveuwtt.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gcplpzcye.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/guizcvmny.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/geaacyyxt.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gynvmsekw.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gizviwxln.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gsrojtwlv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gnwkwdbwk.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gqqzzutuw.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gilyvskfi.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/ggcbbrwrd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gealhrktp.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gsqpdlnku.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/giwvgcupu.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gikdkhesu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gqwzmorvb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gaifucrui.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gszvvmrbl.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gxqgjfzzs.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gztmqyzkc.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gwetjrqbv.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gqjvxenuv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gleajncpl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/goqulfzxy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gffcaboyv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gmnrxhcol.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gbfncwtzi.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/ghcmuhcbu.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gnaykqezf.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gztpxdzxr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/girrdveuw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gtpvctwgk.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gmhlzjfsj.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gkndqgfja.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gbivppowj.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gdqttmwxc.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gfutvxdwb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gfwhkeqxz.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/ghxkqmchf.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gzeuscpuz.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/gzcyylfxc.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gznnylmre.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gypshlzbf.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gutsvfzod.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gbqvesvpp.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gwollwpkr.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gwnvdpgfn.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gjhxubxme.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gjmzforvu.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gswebmmlg.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/guoesrbjv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fehbvm.com/Article/details/gqigeaail.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/grtcfrryi.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtisqjmry.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/geppruosm.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gllhvatbx.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/geqdgjuud.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gltffulut.sHtML


<!-- 参考信息 -->