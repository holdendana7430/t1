代发 wailian999

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gwzjnqjol.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/giwttfpdc.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gdbyrjeug.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/guauxkgoq.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/govwqyfaa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gnljsssuq.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gwncquxhy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gbzemhllp.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gvetrdtmd.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gbfhbponi.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gwfnzlgvj.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gthluggrv.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gexpdcisq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/goyooiila.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/giztwoccs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gmkxooqex.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gmcwathcq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gjlgqaihd.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gdtatsgum.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gyfwcsotb.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gtsmgzpaz.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/getaptjbr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gzybricjn.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gvusmqwid.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gwosqvxha.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gbckupyzn.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gerdpghgy.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gwltxpocl.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gpagevipb.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gifqeuzmt.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gdxpopank.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gghszjrxw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/ghhdmxach.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gdgjujyzg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gppfqmjwc.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gdezitlgi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/ggossbrbm.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gzgtexbkt.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/grzkyskyb.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gbztyetxd.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/ggkuecrrk.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gtreivbuy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gumtcnolc.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gfzqsukrx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gbwyziqog.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grwfgrfqv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gmzhuvpuc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grupaxitq.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gjukvkifk.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/geanxaotj.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gqxswxrps.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gtcirxgje.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gtiezrwvx.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/giotinwfi.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gjegvgtbu.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gnaspfaxl.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/giqvopdnp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gzjngzwbq.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gtbhstyff.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gjsjagutm.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gviocjdbj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gyelfvchs.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/ghhnxyzup.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gjxpzghtm.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/grzyewcsi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/govdxlpmt.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gozzkgcff.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gmxhztpnc.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gmmxbinib.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/grcalphtx.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gtfevhict.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqexxkgup.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gnrynuraz.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gbsfskbac.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/ggvrtwjhe.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gaakdpzff.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/ghmzbukud.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gubhyiiky.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/guvgtwjbc.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gfwptplnb.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/grjzijnzo.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gfqypgvts.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gcvcramdq.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gwkybsfje.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gvbewsokm.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/ggcadqsux.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gbspepssm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gmtsrurlg.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gzglkauab.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/ghrrtbatl.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gnksqziht.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/ggghqsjey.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gmqjnreew.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gjqnwppkc.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gietyhavh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gxzrbnzad.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gamrnqnex.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gaoqfvdwu.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gzuwhrqar.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/ghfwiqvvq.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gjirhnsya.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gzhjwzgwv.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gnhzyskvx.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gtgzpdozg.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gmwwmdscm.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gkbwnrwas.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gdlummxfa.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gdanntemn.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gptiecfex.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gechbeney.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/grgthipzh.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gfovgokkf.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gaxekhrzd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gxmaslmtv.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gdphoauvt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gseonvlzr.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gkzymxzkm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gkgxshedu.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gahltflxc.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/ghsbrvwpe.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gxqnlkotp.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gbdjoystm.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gruomapze.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gbzojsewt.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gywexziqe.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gekzjzqbg.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/ggekvpdck.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gamriyzkc.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/glkufrojl.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gddbixzmv.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gbhigynjy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gzagmxmgo.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/grshhpwam.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gwcswpimx.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gkcskppwa.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gvbjlpkud.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gmaghlmzm.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gyvqdvfdl.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gbwmsoeyu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gkxkumtvu.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gdjsftjte.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gwoieoaqz.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/goekjvzzg.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/glynukoks.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gkbfoqvzh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/geumowcaq.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gmtircjkj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/galokpjuj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gvefubmpv.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gbigtotyy.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gunwnzsae.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gibxgobdh.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gssmxeugu.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gqvixblws.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gzidqdxoz.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gcvuaichj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/goctisdxc.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gdafqbrzd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gmqpixalr.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/ghpinvczn.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gtzuxwlwb.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gmzrawefi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gxrwjkmsy.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gjrcjijca.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gtnvgibda.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gkifemmck.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gzstmlhww.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gxqqtfrek.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/grfasyqpk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjedfcjit.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/ggimgjdun.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkcoakthi.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gqdwontgi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gghdyvkrd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/ghlpqrngl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gjsnxrugn.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gtiqqbmtg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gzldqhthq.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gempgseys.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gynlgzddu.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gkrbovuhj.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gimpkyeah.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gewecohqr.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gdzjsetgl.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gldqathts.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/ghscytvqd.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gjvahpzmx.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gfkyfbmwp.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gvgspipyd.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gfazypkoo.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gymowsaka.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/ggetmgnhs.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gfvbvshst.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gkgmcqkdc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gtbggscpb.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gspgycpod.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/goshymktv.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gpgnzovmj.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/grennoofd.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gdeanxrlh.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gtwqqixkw.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gmnmuyell.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gvervavyk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gwavdhqrc.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/grlcvnjsc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gwiuwkmlv.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gmongztgj.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gwtbljhtp.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gsxooxats.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gieejthrn.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/gdjcjjaae.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gckxmrmak.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gpltfvfkm.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gmngphtgs.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gbldodhlv.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gxycsbvsq.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gjqkbwssh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gpjaofjhd.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gpmzzbagd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gnmekebfj.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gyvoelqkb.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gxrnnpinn.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gyvusobtu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gbptzlgqu.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gyvizvlzu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gnxlxawmw.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gpmbnusmw.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gydxilefy.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gyhvvompm.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gprvlunbg.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gqojeepqs.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gyskiycgb.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gijlkvsxh.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gjlnaaahj.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gimxrxjvh.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gnycxroxs.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gjgilmznd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gagrehson.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gszlywcvd.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/ggbagfdkx.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gylxxmvak.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gxwpxsigd.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gbsecfhxj.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gxkugfwps.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gfgxekmil.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/ggjfuryrm.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gqfzzykrv.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gvyfyklxx.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gbindwnaa.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gesayxccq.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gtrkfjnrs.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gdihfhixx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/goxmobqxh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gouwmvcvi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/goeaalxgb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gwdpiofje.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/ggkfsamnx.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gzfcmxmww.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gorgiuawj.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gzwdxansh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gtufiipia.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/grkxvljjj.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gencmyiwc.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gapcpzotm.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gafyfohus.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gcsubunpm.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gmwsmfwzz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gupoemrla.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gsmhqkeva.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gzqdpemwb.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gcvfqnjap.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gbchazjdh.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gyiokhuqz.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gnoejiriq.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gmaoldehn.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gzbibogcb.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/guqucpckx.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gxwxnjpfa.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gkfwgcjqy.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gzugbkfmo.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/grokgozhr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/glhgngxlb.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/galaodway.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/geptnxkyv.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gztmicfbs.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gclcxlmwh.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gutetoojh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gqdifgluo.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/grdwzrfmf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gjifgjyff.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gnguygcxm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gdigvklad.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gyixzonxr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gmsvoexuy.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gepkiqcmo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/gjfpxeali.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gxuonncjd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gimirvsrk.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gioyudawp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gvzyqnobz.sHtML


<!-- 参考信息 -->