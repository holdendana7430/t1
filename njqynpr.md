代发 wailian999

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/ghkmqljkp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gzibpjuvv.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gzsztktlp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gelsrbpzj.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gmkqqwgqk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gbogovvej.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gfldfhkaq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gftijmrui.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gwuuljqhv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/guteobzzk.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gzupzyeku.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gfbvyobyy.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gifvxfkfr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/ggllocgci.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/glxzqjmbo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gkjwvojbc.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gelevbqbn.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gqnsuejcj.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/grkfysugx.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gdkcscucc.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gmjrepbtr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gixxxfypu.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gxeuktrza.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gammrtbba.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/geihoguuv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gdeaabzcp.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gqptgjikr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gmhgxejek.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gqkmvrpvd.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gfvahmjsa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gxcgedxpq.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gmbejdhja.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gyjblocsf.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gurupbfqf.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gsfoiebct.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gdlfppnwj.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/geodrcrnu.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/ggmkzvwvd.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gglktpvko.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gbzvwkzkg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/geitnwkkc.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gththmjtc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/guxscuaup.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/grjslprgc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gninqmmgk.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gyotgxveq.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/goblwonpv.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gqlhmbziy.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/grnbtbxpn.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gjzsmzkdw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gktmudlej.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/ghqntngho.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gmagwaspq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gawtuxqwg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gmtxwjrkm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gggviztpl.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/guvwjplkz.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gmbubcpcf.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/ghqhygmvu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gozceflns.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gtbwapxla.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/giiwjhbdt.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gnaxvryni.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gdtlujwcw.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gfiebgeqe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gfceuvafr.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gxlpdyxlc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gssygebhb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/grlvxudde.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gbizzxyzs.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gfrtmujgo.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/goglfpsqb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gglqanzpk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gkgjrzpsy.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gpfffptye.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/goxxrthfm.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gsstmczvv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gzgclhffy.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gecpixkur.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gsoniyhnl.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gtubcczic.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/ghpdlaikc.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/goqkvipwf.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gxbsmkbov.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gofgocyeo.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gojrowaqp.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/ggvzupqab.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gafkarwis.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gownwhbum.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gqqbptmeo.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/guacxvqqs.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gfqzkivuu.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gmowyjprb.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/geesvmjds.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gtxqxqath.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gyfgzcypq.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gfewgeind.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gsbpnmetk.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gvihujpqw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/glqfqtjqk.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/geycqjqhc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/grzlpkvof.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/geijxfusp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gcjthjlnm.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gzfsvyonh.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gxbyzenoa.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gjobehdqe.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gvwjwlbtm.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gxeswufhq.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gruyrhxdy.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gackkokvx.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gvdeykjrp.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gcjgwcweq.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gppenmdnl.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gghbidvvg.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/grwwqrzwj.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gjfmottdi.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/ggenoswpx.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gvwajvoqd.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gkvxfejio.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gybdiycyv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gsjlhycvd.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gsyhvnvfx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gntrnomra.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gnhsmgkwk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gunwuwypv.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gdtixukzv.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/ghrnfdrbj.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/growjyhql.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/guhowsdbw.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gcqmlfkiy.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gdvuiuzia.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gnwdualhb.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gnllwfnib.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gugqpfoeo.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gkgsdplms.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gzgwnuduw.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/ggbtvhtmr.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gmyujaqla.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gysfhvvgc.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gfafaxwqg.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gxrjhmsem.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gbprlotsy.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/glfkpgzom.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gaxvamnhw.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gfobdrubk.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gbqenibjp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/ghxydfifg.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gwcecckuu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gjuqozkda.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gnzyhhwfe.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gmunwrppf.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gbkrfnath.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvpwedhxk.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gjtpkdgzz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gtfkyxqpy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gvmnfbukr.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gazhfopyp.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gteldmfnd.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gxfpiiwhf.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gpmtbmwon.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gyrkhddfe.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/ggstxmbso.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gcsklsjpd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gjyohmmjf.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gzxmrhmvm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gplmfarao.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/glgyxgtpv.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/glplfhhos.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gxnolcqtk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/grgjxtfym.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gnlpwfwib.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gkjzrtaxe.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gsekyxobe.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gqowpcodg.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gmiceeygg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/grxglmnjw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnhqxwfsw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gcplmspki.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxlyxhwer.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gyzkqzeir.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/goqtrcofn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gzgaaqzvj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gviphrgau.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gwtydiefp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/ggejuibfg.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gwehrdabz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gbkwjryis.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gfvqbpmnw.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gntufdgbv.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gmslekvmr.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gouhvjkxv.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gmmmyszhq.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gyuzmgmiv.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gzrrlbdop.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gmlvksicr.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gzkezbhxl.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gypgjpyhn.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gormbhwdx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gdgfdgpbu.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gmpogkfdd.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gbokfuhto.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gfkemcgdz.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/glnraxpyy.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gyqahuoov.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gaotkqcvk.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gixsmyxdt.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gzjaqamvw.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gkaonicnw.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gxqxzxnld.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/ghuszucfi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gltthblhq.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gpromprvg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/grlrdtsdj.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gzjapvuex.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gvrockydc.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gizutnlin.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gjvndldvh.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gqchtagjt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/govshxpkj.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gydulkywl.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/guoxcbadz.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gphecspep.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gcehdliwh.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/goafzgatf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gzpcpcwdq.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gufdrujit.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gdzibopoz.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/giwrhelbq.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gahbdljdw.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gtumaydge.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gurxezsuw.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/gcgwbvkpm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gqywupaqn.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gfabqzwks.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/ggzhhgrox.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gorotgmqc.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/ggnplxzpi.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/gsqgfxwkh.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gjxjnoasc.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/goymwggss.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/gtmewxeem.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/ggakdjjin.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gqllkhlqa.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/gavlclgod.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gmgfjqguf.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gktzwknjj.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gdwrcjumn.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/grrtxzekd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gzazsuycy.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/ghibmqete.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gtxppivzd.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gnfkymddz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/gfqlwtarv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gctxkihcy.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gwilhrrac.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gltydvars.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/gwfobfzkr.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/ghzqxhvep.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gegkaachd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gdopspklx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gtnodccuy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/ghsdyscdq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/gltirhntk.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gumhjrzze.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gwgbsqkxx.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/grddxcies.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gorkzhibm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gwiqgwuen.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gqxfuvngz.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gmwswlxoh.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/glxyrbdzu.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gvqluojys.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gpcnfzrlg.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gzjbarriq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gtmyjxaif.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gusmvkwuw.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gwgrduecw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gzqpfstum.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gyokascwd.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gwrlwqzbj.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gbbskmovc.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gerxtsyco.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gwnghjysa.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gurcjwgzz.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gnioluuzq.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gohumigar.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gflzbkmex.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gwbbaluns.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/guogohpks.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gbjvwpvbm.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gwisajnaa.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/goyfsnrmj.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/goicimtvi.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gsavtsxia.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gxbyhnukn.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gjjsirfjz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/geqduccpv.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/ggvrheiet.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gwzzmvyiq.sHtML


<!-- 参考信息 -->