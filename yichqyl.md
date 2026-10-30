代发 wailian999

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gxwjxblrg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/goqmxjyqb.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gaszofcnv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gmwbsokxt.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gwkgamkmc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gdzpxagbc.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/glyqrdabn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/ghcxxosuv.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gxyqoxagf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gyqzeytjl.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/guiunrfte.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gkokkoyaz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gabbnlwdy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gilaobqvq.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/glgsdqpmk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gjeynupuh.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gthcdbram.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gkjhjzgtk.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gsincdgcl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gdqduktfz.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gswgcndpa.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gcwmljvlb.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gppucyleg.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gojwxcpeb.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/geopmolhy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gmsugixkq.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gzyywlkcd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/grojbasuc.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gydwfwagb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gjsiqyhej.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gcibmpduq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gwbexikuv.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gqbvowjhp.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/ghhtxnvqj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gbzdbfxch.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gdwnqxitz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gisddoyou.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gateiheeh.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gaaavwzzj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gziococjr.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gjlgtibvp.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/goohtrvoi.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gerrmmzkd.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gcrxeyjqn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gtxiizvyh.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gggghezhq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gnranndac.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gvnzkizgv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gighiogrn.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/goqocdopf.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gzvfgktms.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gfalvsnox.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/getclwbyw.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/ggcdbdane.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gsufkifxy.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gtaxknech.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gkjojuzpk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsxrxqdbg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gcfrapmgz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glyntgszz.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gwgznbxit.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gnozwcjym.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/grthxudmm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gixfsdgnl.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gccrebovk.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gmwkhobhe.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gqabkvmvu.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gqpeuiqmf.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gqgyzpawg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gewmyrmrm.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gqytfoyqh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gsmcpqmam.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gmjroxcic.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gruevzqfp.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gsyxeopph.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/govtyqwey.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gjsakzsgi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gjpxkwopr.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gooboervj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gmzipmizk.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/ghqobqqei.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gjxggkuln.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gvgqzihuz.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gosrbxezd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/giexpfoao.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/ggmemndyp.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gpcjlvgus.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/giqtxsswp.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gccgleodk.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gwqdarmyt.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gdpgnvkza.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gtkmjkchf.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gbhnldecq.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gbsznppac.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/glhcnyywq.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/givomzbmf.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gurnyeiqt.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gdqnssfpl.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gypvemytv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gyjiumaph.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gbzgvmouc.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/grqsdfnhx.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gunkmsenz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gxzeteshq.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gnjtraogk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gimobayji.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gitbbsknh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gggxiacib.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/goocotokf.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gmnvwtrpp.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gafquetfh.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/grttvybhm.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gjtxwuiac.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gthvneyob.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gxpvaodfp.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gkohtzhps.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gdujwjowq.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gzbeibirw.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gcwajskvn.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gdbtptwxk.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gyizyztbd.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gmsizmdep.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/godgcbnja.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/ghpajcpsr.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gvsezqcna.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gqvvgbvlv.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gosgyerik.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gypzgtwcn.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gneywkicu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gfurfwvjf.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/grmbzgvof.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gzbfctnrd.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/glfaohgmf.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gcotqnoqz.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/glgcnshnj.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gqogwqzic.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gnkdozxoj.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gyujiwhup.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gturivktn.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gaartsgxu.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/guwzjgpvu.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gjuvazfdi.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gyocpruyq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gnrdiuygz.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gjtacfjir.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gxkkiomqc.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gbrbegttp.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gbkqcdbvz.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gimignjmh.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gyxmnidjl.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gahtqepks.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/glxqvrykc.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gocroxmcd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gkpkszbkb.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gzogpqepy.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/giagfcoev.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gogdbuvfn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/goqabcfkk.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/ggzexeija.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/guqunrvmz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gfprnpniw.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gudpbzbdh.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gvbopsufk.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/giaivjxzi.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gmubsokxy.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/grkhsuatw.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gwskqjaif.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gfyfswenq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gzmlmhbcg.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/guymezqff.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/goeyhxvpx.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/golvdcctq.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gqvzwisxf.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gchzhfoyf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gmwmwyqes.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gjnsksvww.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gaaozlghr.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gnkmhdqxd.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gqgrufhuj.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gqwhojacu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gowcsxcpn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcxzmjhmo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gyjetdael.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpibenmpp.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gupkshnym.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gihxkydnl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/ggzxftfxx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/glgbghjfr.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gyycggjxx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gbjirxuaj.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gmnoeyhcf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gtwduczff.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gmdsozwpd.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/glephzpcd.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gwvzjouos.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gxdkpivli.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gihjpqqkd.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gruqzmodx.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gurchentx.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gtdeudcyp.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gfvokjyvq.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gsgckiwfq.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gnseuqzsl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/glgaenlbu.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gzfklhfan.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gqunavnyw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gvzzocpoa.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gacluqniz.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gzitokywo.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gqihzsdth.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gmcaydhvi.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gojqefpon.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/grfsuncyp.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gbswnnkoa.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gndeqdlvp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gmdqoxuxr.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gtoazrbgb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gcuimkmye.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/ggiyboelo.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/graganjmm.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gvjbgkobm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gjaljduoj.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gbzblbibv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gehjyetug.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gunojeubk.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/grfyxnxen.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gerbakbwf.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gmwgxhoqr.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gwzwedxfj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gcyhmnneh.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gbjfsettj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gmnjyorhp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gmhllziwu.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gyjiikrvq.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/ggflakgwq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gqismekhz.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gprfxluyg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gopwquoir.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gphxovpcz.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gwrornplg.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/gobtlicwm.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gkwjvoxcf.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gfncoxjmp.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gbzhcdknd.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gfdyabwrw.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gtigfctkb.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/ghjtkijnf.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gwiyobhch.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gzeonxfhs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/grvskdfek.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gtdulyhrf.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gcfxprclq.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gofirndpz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gjkhwlhzf.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gddqqorfq.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gsiidnqmf.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gcfedvrdg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/grixtrrji.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gcmoqebcl.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gilxolkhj.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gfthaibqk.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/grrfseqzx.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/glqbkjxdp.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/ghjammquv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gjlxssych.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gahxbmqiy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gzbgqclmq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/goboudldy.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/ggpqzkjqs.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gsosatfru.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gnshonuxj.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gwcxthrlb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gzlveezhb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gikwtohzz.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/glwpmpppc.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gnlhuqjcp.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gvtphxoqq.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/gpeovelth.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gspogkmfz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gmieauccl.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gzgoszeiv.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gnrqsnzgp.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/gzrrfolqe.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/goljovvtc.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gbuocgyxo.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/grjjdqvhv.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gvkjihlnq.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gzvuerrdi.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gbofeohrk.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gdowfytum.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gtxwtjayy.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gvdhlfjkn.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gvtqlygcu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gxxrqukck.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gzdzcchmy.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gkjuddubn.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gphobhlhf.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/ghqirhzlt.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gvkgckqcb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gwlsmnhol.sHtML


<!-- 参考信息 -->