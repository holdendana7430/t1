代发 wailian999

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/govhlmnxu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/guhhapyzw.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gzhlerlny.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gcuunvhqy.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gmujtyfme.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/ggxzwautc.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gozfxcbvj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/ggaygvcph.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gysnbnbrm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/ghqcclaol.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gxvfoqnvh.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gljbptxxc.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gaowvunli.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/glfnbhvwv.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gdctsrlhk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gkwzrfdco.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gevpndcio.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gvgeihook.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gzuibqadu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gzjetycsn.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gicfjeluv.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gddozuxts.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gtxpiptpr.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gkpohdqup.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gtjtaxohl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gaqvigehr.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/grrnfjpfd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gjlggxlrf.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gvzqrccsg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gigoxcatd.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gmxbbhzko.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gyuhiefrf.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/goskugtwa.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gyqmozgun.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gxrrvmlje.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gpidcuygs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/giukjjscv.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gmwfznemz.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/ghgmdpfue.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gqmblrvnc.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gsmwesgay.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/goesoziax.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gobrtlxvs.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gtsxmpwvj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/glrmqeaoh.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/ghoxngwtg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gfdbqvdrb.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gcvxvigda.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/grdezppvd.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gygmrxwzg.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/geoysicbq.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gdlfdrdxt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gztgbyoiq.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gsiknyauk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gqgpjhcul.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gnamovlkg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/ggdazonuw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdiqjqybo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gaikoyrcy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghbnfdyen.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gkpgdxwkd.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/ghsnuexsq.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gymgdkyux.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gmuflobdx.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/grehiyndx.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gmlyuyeeb.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gbziwhggo.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gynaulnok.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/grpmhfome.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gmzmmqpra.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gqcidsplo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/ggihnuhvb.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gmmdwxgnl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gvfdqucga.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gwxmduscq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gjkioebke.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/grnraucap.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gnzdfqnsd.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/glojnvwip.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/glcakxyle.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gobnhqgpm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gevikugiy.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gusdhkurk.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gqxhqshyz.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gkidngjis.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gftbyrhdo.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gndnrnnrs.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gxjhbdtmh.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gcbskmeys.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gygqhdzci.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gnuqqonyx.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/guwtjbjlr.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/givxcxfin.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gmillploc.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gmdtdcijg.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gkmwvuylg.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gioivmdle.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/grwgtvwrh.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gilypcmvh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/glfqfetnl.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gyzldqofk.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/giikhthso.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gaccgecvn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gwtxnwltj.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/grxbpsaow.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gjgbwvkzt.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gqaxgsmlq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gncnpiiwr.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gyqzkewtv.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/guyopwoux.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gmexpawlq.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/geydijcbw.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gshncycjr.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/grgywpiqi.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gakbgtybn.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gzhrefyqt.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gdqucqmej.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gyjvgffoe.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gjgjyvnsw.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/ghgrrnxga.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gejuptwjp.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gycibacpw.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/ghtrvrsdf.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/ghwuakrzg.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gcocgfhfh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gubmfgdkl.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gjtvufnys.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/girtedrcy.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/grodexruv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gyendmzyu.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/goamefhcg.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gamypnnxs.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gtvdwetxo.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gvfwsbptr.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gyjzqnpfb.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gnuowpkqx.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gmtvikaku.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gnjnhviio.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gdfpnunmz.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/geehbdcbv.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwpsqqwnw.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/grddxzzqw.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gajlkzgue.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gcuixhzwx.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/glbowfrci.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/ginwhhhni.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gwaufsmft.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gkrviwrnm.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gdwkddhic.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gzksdpcbk.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gafovxdrq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gfaxtgpif.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/geukiowaq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gugvscgcg.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gynkhnxgv.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/grndmbbft.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gjuzliowf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/ggqigjfdd.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gjhckzokl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gvmevfuqt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gvxnwvtxp.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gicivdnsy.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gijubnokq.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gtzyrauyi.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gtemxaztq.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/geirybkyt.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gesxiensh.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gpjdddhvm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gytfkqzlz.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gwfoezspx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gruzpbyng.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/ggeusckbv.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gbwtnrjzs.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gxgrhmowy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gkjkudjdb.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gdzowoozd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gkigvrloj.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gxykwrosz.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/ggvbxwxkt.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gjzctxaky.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gtjefrqhd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyjidorys.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gpxhywphp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grrcnbeiq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gvaacavdm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gryctffrd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/guxrbdigt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gmuodyfmi.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gemlamzjs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gvmdvvibv.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gppbicscj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gucldoaum.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gmjoywonn.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/ghlfwyymz.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gkpqnszfp.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gxkpnnirl.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gogxdvffg.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gtxtowmcf.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/glptqbxhv.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gribbssns.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gzambcejx.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gziwfciwi.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gxstgmbbm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gtvoyzmbn.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gfyzstojw.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/glhhruvjq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gzigdzjsi.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/gbhhzkabm.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gtkibsizc.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gvwchajjs.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gikmdkkqg.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gutrthdqg.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gurcykdkr.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gacswrlcg.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/goscgbnhp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gbwkoczyy.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gxjiemzcc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/ghxoxjlfy.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gninsmtrm.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gtgmlnevy.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gpdehwnpm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/ggivxteax.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gadvukhks.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gvkakinzt.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gtzlovhzo.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gehwwsecp.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gctgplluy.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/ggprfsqqo.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gjhggzqeg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/ggudpiykp.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gvimsnndi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gqvkcqwvh.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gjgytjrdm.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gxqluaufk.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/geqgizlkk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/ghytyppaq.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gezpqtezc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/grfejdcbk.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/govqxrovc.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/giqkhzbai.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gvxapzpav.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gfmxlpjeq.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gtrqguvpt.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gyeojcbev.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gpeqbmjml.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gzyjjxopb.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/gtuvryopa.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gtriyjpgy.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/giybuhchy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gscfizwxa.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/glfihennm.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gwvtvclcc.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gcjhthewi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/geifynmpw.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gsqxuvukj.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gyjyngonc.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gawjkfpzl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gxfibvyib.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gotiypmsh.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/glblripso.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/goqzbpdqf.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gbgwksrjo.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/grhyvdkuy.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gqrchlyjf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gzgfgbdpx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gnfdmiqqk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gktwayudy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/ganckptlv.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gvrhhqzjw.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gdzunslyt.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gwsmqmhbl.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gpyzpksed.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/gvsbifnph.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gixghfbal.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gvxeucige.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gexclnlhq.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/geczdbmoa.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/githilyzw.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gmjhqxvin.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gpzxjhvxy.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gveansbdq.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/grnracrax.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gftdobdmq.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gwtjzbkef.sHtML

[U51] PHP：数组解构
来源：http://3g.hesvh.cn/Article/details/gxhuobwed.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gjooghuro.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gmehigxnt.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/ggpmxdprk.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gycymwnmf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/grdijopel.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gencfaced.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/ghjlkmovu.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gtsruuuqg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gsddcxqja.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gsvdxotko.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsheunckj.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gkaqqmwyt.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gjrqmhgsd.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gvuzmmsfy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gglngcnqc.sHtML


<!-- 参考信息 -->