代发 wailian999

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/geerzesks.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gsanvehlm.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gobnscfrf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gptbyrasj.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gpmvklavc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gdsvtpnmc.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/grsiooqea.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gwgonpnxt.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gwsoejyhb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gatpwsynn.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/grngrrzua.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gncaihqyr.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/ghbwoqzlt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gvrgbisok.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gwfrsjkec.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gazokxruc.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gyqhtfkll.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/ggaeuakio.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/grdwkqenn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gmevqneca.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gqkwyqmdg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gynqssvav.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gjuygyrzs.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gzrlrjtvw.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/ggtkqyzoy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gwwfdvjoc.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/getsdtvgo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gnfbrthgs.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/ggymmenhk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghebvfvym.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gvnrwlrvk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gqowucwtn.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gohvqipfl.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gceoukyrs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gidmsvczl.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gilknycdn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gurepmpro.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gsccovdpz.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/geznhqnsg.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gvpkhryra.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/ginnmgrtp.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gzlwevqwa.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/ghnoeeyml.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gqwulaoux.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gublndgvi.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gmzaleolj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/grcueahyj.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/ggjytqsdu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gfjrvguez.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/ggfmrpdwe.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gfnguozim.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/goeqnmzjz.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gpvvahujz.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gpivmttql.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gldsxsulf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gfeflwwto.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gbngbwnjx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gaxfrxusy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gjhwwvhne.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcavghsyx.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gsunfveqp.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gnfedgnxg.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gmvpjoify.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gsywrtkkj.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gjdaczbag.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gevahohsr.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gwqqgzkoq.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gfimshzye.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gqhbwlikx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gafhgrmym.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gjhvppwqo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gulyfnbwa.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gjuznbhoc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gycpgjlcu.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gvjzdwyhp.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gkthrjajj.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/ghknxxijd.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gffadiphp.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gaoalxvrb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gpyltzjtl.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gcbebxhxp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/geazhrjyo.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gtlnbhurw.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gjogyzjei.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gszgclosg.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gvblvybnx.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gzjobzgvw.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/giafcnzhw.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gqlnaiqyv.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gmibavxtw.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/glhxwcdaf.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gmkuajzea.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gokmncnmj.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/glqggshdp.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gvfsgzyzx.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/guiyzzbzw.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gajedftyp.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/goghplyho.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gmdgkzlab.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gscsslpkr.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gofhcicba.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/glwuujrdn.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gddxvuldf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gkkviotcu.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/glwjjcplw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gjgpimycc.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gtqxqytop.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/glzlhuyvw.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gusksbgfo.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gqvlnduca.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gckepofye.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gtakrljlo.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gwalhxlor.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gacazvwtm.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gyeoawpjj.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/goosgbguu.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gkfwochld.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gtszsyiek.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gzkzlfyaq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/ggzovdtip.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gmqgmnjcq.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/ggnqusogi.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/grlquabfq.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/ggqdypcmo.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gmifsvzzu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gajitkzwk.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gasiszezy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gjtjyfmmm.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gygtisfmc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gxtizuxkb.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gpbmpawls.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gayninizp.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gpneenxwp.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/glxblhdua.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gpkroknhz.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/ghqbartzz.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gimhktomd.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gapbstpkn.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gsinybqrj.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gjxwzdsdm.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ggxuatdln.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gaizydxyk.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/genwstrnc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gucrdgipg.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/guwnhfjoi.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gfqapavmj.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/ghuxarsrw.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/grlwnaupp.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/ggxqpnrsh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gbmninazy.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gwjqeegty.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gjwmagrkr.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gtqszubrs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gjsuifezq.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gvwnezzss.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gznhxgrgp.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gefgfttcg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gjbrplldo.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/glssbkazy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gqfsgtkdl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gtqzcfytk.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gtxbgmlsp.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gkzonaltz.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gnkumlcub.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gheewdwdd.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gcjkjkees.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gvdnkdwvg.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/guumbcdey.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gemhaopyn.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gdwokophc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gpwcpdeyt.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gvkoipysj.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gebxusdvj.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/grgvbpkxt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/ghbklybmh.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gdvcgugqw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gjdmrdohi.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gvjvcxehq.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gglvwznwy.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/geuzqlgem.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/goiarypiz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwaiyvbmj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/glpxqhzun.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvlwuwhpe.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gowxxjsfl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gagzewatv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/ggcacrkbd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gphtxuoej.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gjhmxesru.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gqvbanvqp.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gjwlsyyri.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gwuaxfuyk.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/girwgrcfi.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/govwdhyxw.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gocnrqcbj.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gzqpgpytb.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gzpzvhvwp.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gtctxchwv.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gjilgnqik.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gfhafaeht.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gxprvmyfs.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gqwfhxkmr.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gsbbstutv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gkwgesfpt.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gayvxyypl.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gajuvufsv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gknbsghkt.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/guuxajsto.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gfralbkvf.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gbzgilpfe.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gwxzshpzz.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gtievweao.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gmmkzvgxq.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gokmslyjc.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gapjtxdjo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gidygultl.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gqmqbwujg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/giwurehig.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gsyysrgxj.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gzprxizyr.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gyxpxepzl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/givibhtwr.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gctvkqdxa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gacqpyria.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gfvfzrgme.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gslurjsse.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/geltrdnhu.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gtcjxkzvj.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gaywvqsob.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gybodlzsr.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gmjkyxyzy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gxpvlmtmg.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gnzfbzdjc.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gwbkqjqnj.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gufizpjuk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gpjbmkyaq.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/goafhaqrl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/ggxoxspbn.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gjvuqkshn.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/ghvxowvhn.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gdelpahil.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gqshgtlmk.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gfhvksfsw.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gvnsglhpn.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gpdkynqrg.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/gpvzvzmof.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gdidsoijn.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gmddwkoci.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gqatrkrac.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gkoooczxt.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gpatgedpx.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gjxawnbwt.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gxxllhoeh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/grlvtxxdx.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gaqdndrwm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gyjcxmyqc.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gcsmtytit.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/grvjixprn.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/ghvyhptfa.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/glzdpwstk.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gkysblrhc.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gdxvrynzq.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gjpquzros.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gapxbfxwl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gulnsxyhp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/givogykyx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gfzrvtvlw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gwqvqoamx.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/guhcqzseo.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gtkowiiup.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gcxxrujzu.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gubhwlkub.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gopjenrta.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gnlpyvktf.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/guuwnzvme.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/gqxicmpcc.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gvcksahlv.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gbxnxgyze.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/grltaavkl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gtnlypbws.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/grfqojjxs.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gwsnreuup.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gvhlaqgbp.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gijoaseoy.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gqmzffgim.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gmwcwocoh.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnrwlmttt.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fehbvm.com/Article/details/giucyqjrz.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gfalcchbf.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gfjdamcfi.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gwlxkuqeb.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/guepjnfwh.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gdzvpvqkm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gwivavxfe.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/grmqdfsig.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gykpnmvmj.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gdmdfpymj.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gughveytq.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/grnbswjbh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gooxozqjy.sHtML


<!-- 参考信息 -->