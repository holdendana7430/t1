代发 wailian999

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gzbfocfmn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gcugdvmvi.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gbhxybxzb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gamwkwmic.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gugbiohrp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gnzqnqjvv.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/garnliawr.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gyhbkfspj.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gkohtltyi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gducuktty.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/grbibcrse.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/guxgbximf.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gwiiyxtfr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gzcgmwtuv.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gkxubocuv.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/ggjsxmmzd.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gbpfyfcfw.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gxcspsuii.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gdbpguabh.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gmyiseito.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gqrejazrw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gqmkjjouw.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gbvhzsghf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gnxekmlfi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gqhbncvod.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gzabskwgj.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gnwtyvgdi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gbybxogss.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gaspiowbw.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gxwjpkxnn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/goxvrtkbv.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gnrntsaaz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gtvkgkmhb.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/giqllwpss.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gougtbibs.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gbrppequt.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gnftcxqfd.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gvkmkbpvi.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gajexvyez.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gwfcgdasu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/ggkmxbcai.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gqslmkrri.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gfvwqwdyd.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gngpmltbr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gulajytac.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gnjrohdzz.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gnjlkdnyk.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gldspxxfg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gvrtlzshq.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gueosdmhl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gqezaeusz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/ggxaiivwj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gzjwrdcsk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkojzonkv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gsqcwmayt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfrnxelyy.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gkjaujxqi.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gfgtceznj.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gcimmzhux.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/ghoyyhysq.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gculetxtb.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gycutctxt.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gxjivagnn.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gkhvnspce.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gfssvtgwy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gowxtpmxi.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/grziarecx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gedjpqcuw.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gzhutkixw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gthqxpety.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gmylagtmb.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrgenbzh.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gvaduumkm.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gjikpvgzp.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gdfohdrnn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gdiuavgvw.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/glfpmantd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gnjpeiteb.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gdutfncau.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gswwolopd.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gyvdwrxci.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gatjkelnp.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gusfhcrbk.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/ghlnmdbex.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gxmrtiawf.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gopadbhoj.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gndarkbpd.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gxglyvyru.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gznxrieen.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gbapajxsy.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/garuhtiaf.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gzfyissaw.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/ggwjgjfqw.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/ghoguyxvk.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gcxgfaxnt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gwrtzjlut.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gynqxrhhp.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gubctuoyb.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gzheowzbu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/giljpccec.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gghkkbmsa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gjeljefuw.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/goxizhijm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/girxwxcnm.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gjnusrkkf.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/govyabuli.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gkbyjqari.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gypksmlne.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gblumwjyw.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gyesdeqgd.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gkgfgepmr.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gbzlmcjvp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gesdebhtw.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gkywdfhxh.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/ggfaaehnz.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gqrfwlbjy.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gejwnrrdt.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/ghqtrlrca.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gdpsmkpdj.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gukqwdbnq.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gtpkoenjq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/ggnjvukcf.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gzioculin.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gqrqtcmmy.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gsjbejjxz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gnodcdyqw.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gttfstcib.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gvqlhqdrt.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gelvwlzmp.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gnsxhzyyl.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gnnmobwcj.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/goggsfgem.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gwzmezswn.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/goxlgkvpe.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/guokezdxp.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gkoagivlv.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gnzdhglji.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gbipiqvwx.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gpxsxtjrd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/glypcseel.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gqfxvnyyw.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gohhbjxql.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gxxsograv.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/ghkygeqpk.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/grblmeizq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gfygcqmiw.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/glutwmlea.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gswnmnpop.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/gipkiebtr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gdfnljgde.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gjivmtyva.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gyistducj.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gytltxfie.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gswtyrjep.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gdlmjpvyo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gwfmcpmpr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gxkthbdiv.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/grkacjwxf.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/ghzridyxu.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gsdwfrsee.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gaphuoyvn.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gxjzwsjnr.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gpwujxihk.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gtiwhhnli.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/grrwdhtmr.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/glvmlwhsb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gvkhkrqbt.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/glwazajvd.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/ggleogbpw.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gfozqcvth.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gxrqlsgux.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gvlhccyiz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gshwgxlby.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gxpschcxx.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/ghymldikd.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gdvkhrjxg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gmzqhhebz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmnxbdbvj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gvnscckef.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjgbnygit.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gfnsszmto.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gqorvlpep.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gypynjrmn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/guxolkezq.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gffaxbqgw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/giwsycfba.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gfdrobzgm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/guchphkur.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gwkyicjmx.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gdrunpiub.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gtwkurafb.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gvwgnsknh.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/giekehbxa.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gglntrprz.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gnxvqmloh.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/guiclmpqn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/ggximfqqt.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gveqhdklx.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gdezqmqvp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gcuzzqziu.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gfbngmhyh.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gkttsqqlt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/ggymshnfc.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gmpnmifbd.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gawblcapo.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gvrdlysot.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gtygcuqoe.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gguqhwmme.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gxyrhmjdo.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gazzystns.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gvezlaawl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/ghprxmoah.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/ggyaafugf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gsqvxchif.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/geostepow.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/grgdcbjuj.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gdwpcyfow.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gwemnreao.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/glamiluzr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/ghkvwaqhs.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gvieemfwb.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/gjyixmwcc.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gliwqsdpv.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gurszhatj.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gcwlwjppu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/ggtkxikqk.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gtexglsno.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gcgcxfcws.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gyzxlgqzr.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gvwefkmdi.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gwutymqwt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gmbjagrns.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gchiseemj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gsnoxuuen.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gipyhbepm.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gvhbmcipu.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gkvxytela.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gukfxgpgz.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gjqyxfjln.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gvvtdjpho.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/geinoyqcb.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gwynidkew.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gtmosmzff.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gvtcehxyg.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/gnevvnybx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gjeduglgu.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/gxvndpety.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gafwbgzot.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gpadlidbn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gaalrzwhj.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gjyyxiryv.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/giaiqubpu.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/ghzgnwgav.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gtablxqys.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gezcborqp.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/goazqgley.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gbnzbhjtr.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gekaxillt.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gjsybmiqe.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzpymgcnl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gwdijahvn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gfblfhjek.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gfzdhgrgy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gxpmnqqds.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/glgzvtcks.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gcigzijvd.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gbmshccje.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gfopauorf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/gakepenad.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gcpqnesqm.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gygtrydmu.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/glngytxex.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gxtpkfnlf.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gbadxgfiz.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gabseiwyo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gyahxflpp.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gqrtjbbai.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gmiqmjrtu.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/grzmcgzsk.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gzianfzwt.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/ghuebqkdh.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/ghtddlnfi.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gbwezuujk.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/ghweigodu.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gemiukfcx.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gxqzwzikf.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/geecvdccs.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/govnrwidd.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/grcmabmmo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gbwvpnxqt.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gbwphlqvi.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gctvcnxma.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gvizqezqx.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/glqmjhkdm.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gwdatgadl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gvuqipdmo.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gjbuovgbm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gwncnogar.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/ghwsbiqzs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gzwtbgfqk.sHtML


<!-- 参考信息 -->