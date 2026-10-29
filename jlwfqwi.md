代发 wailian999

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gvqyhqycw.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gmujnlahc.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/guncbnrzg.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gknhunfjp.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/giuwmxnpk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gbtzlypof.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gkjyyncgt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/ggckqoegw.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gldroovsy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gbnaunptf.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gbrgxypkg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gwvjvpqwj.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gbvrprrij.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gokhquork.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gzkvbcpgb.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gkmxashoe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gfgsmhmru.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gsomskfmc.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gokkfbjsn.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/grayfyhrd.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/ghzfvpjtb.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gztyyjmcn.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gmxfbkqfz.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gxpibexpb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gxwujmibz.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gwjkqvxxf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gqnyakmmj.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/glapataqp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gcnsygmgz.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gygjchaiz.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gzqcofzvj.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/geglumisy.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gaqmefjqj.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gocoiirdw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/ginpdiszp.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gzxilpksu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gscicywib.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggvwovknn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/grgntmigw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpijxhcuo.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gldenfsny.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gmhhjwiqn.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gwdjkqvsn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gpamyocjr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gjahqpysf.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gynhcinos.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/grsdjgvqf.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/ggcikziai.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gvmksvfny.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/grghrerxq.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gwrvcjihi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gaykqmwrp.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gxawylwoo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gbzwbxhdy.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gmdmxxfvr.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/guycxsxsx.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gzpddqzrl.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gvuodsezz.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gbkvjtnqp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gwvlfczyd.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gadyuyetk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/glqntskkr.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gluvwgovp.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gjihtwsee.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gjxujbobt.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gzsvrvrqj.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/glfnxieqp.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gybojfiuw.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gkllhnhro.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gnwcmalae.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/glshpnphz.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gybmsxsrh.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gtqalfbts.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gsvvqkkwr.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gkecbdxlx.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gzxthacqx.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/giczmcxqu.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gsyiqcsdm.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gevatxmni.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/glvwmtjsi.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/ggessumza.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gdbmxtzns.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gedxtruoc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gqfyagcso.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gboaqqtgn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gwuxfzyke.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gdgqozieg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gjxriwaro.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gbhgpwjuj.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/glhwnolxq.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gdjwbbbpz.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gthcvivvi.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gssqtdjpm.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gsagxqkzv.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gbebafvzb.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gdrgoxmni.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/ggtemilhr.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gcpyhavme.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gxydbcmlj.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gudephydk.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gnggxzonv.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gfuolsgff.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gcdczgqjq.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gmbukvqev.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gjpqldqvw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gbhogomms.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/glnpbdcbt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gcpnmibgw.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gxynbetlf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gjuloqepw.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gztetueww.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gkauvblkl.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gzxffmuez.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/goacteqdx.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gcdnaozjw.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/grqjipcms.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gkqpmreta.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gybplyzom.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gutbmvrzq.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gjazspwft.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gsssvvsey.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/grzxozzsc.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gpcrfdiml.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gvwadzatg.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gbdnqyfcg.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gmllisjqu.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gvkcjqidk.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjdpzybhs.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gymfpavof.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gjmfpsrgu.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gawmavyce.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gyzvezzvu.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gtrkmtuty.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gkuufgmxz.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gbafekrac.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/ghjjglerc.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/giwyvxoqb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gncokfkee.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gfvhowhxz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gunytuxwe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/geksulwil.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gffdakyvu.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gdsaocxcv.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gdzvuyqnv.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gzbdroxkk.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gnvazwstf.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gaavipjda.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gbatwozno.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gkargxxzy.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gpdfnoctt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/ggklbbbeh.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/ggwtgclfq.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gfbsxtysj.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gupystcwk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gheikjpyx.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gmdhtmlzc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gwzyzlhwb.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gmpvbovtk.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gnfaodbpm.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gqftwnwyj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gsgkshuqn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqideunng.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gokwlzmsr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfbtmobfv.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/glvsdmact.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/goicqzbpw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gdpbfltzt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gypvnplmi.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/ghubiwtxo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gszkvruit.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gubvhzzcq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gabelrluy.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gugrhscjo.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gbcoplfyh.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gfuqrvciz.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gogxsmuvo.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gxxukllub.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gvtsizwjq.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gbrhyhmpd.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gaddzmoyn.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gkivtunuf.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gyfkrwstl.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gdtvqxrao.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gbnibbkgm.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gmauxvuah.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gtnawzcxp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gwapragph.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gzgatgzfe.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/glcvohsun.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/grbxpjjpc.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gtiflgtve.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/grxpzcqnh.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/golsrumzm.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gwjnxkcmg.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/ghrvsuium.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gbbaofufk.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gbkoovseu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gqgisrcju.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gxmuoqqkv.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gniwxisiv.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gmeplelom.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gcanyzris.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/glqshdrmg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gweiwjxtm.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gevejebmu.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gojtinsmo.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gqhpqdxas.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gxajoieys.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/ghudktwlj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gtbugmiew.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gjrjyidnw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/goidzwcsn.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gfgashgmk.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gwnfpvtap.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gdmttwcoc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gbiporimj.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/ggnvdkign.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gylylydqa.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/ggzwiisda.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gpyzermaa.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gpgijewmc.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gcoajlufs.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gochmubbj.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gkdlrochu.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gnekqsarx.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gudvnhhpj.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gypocdutr.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gbrwwgzjs.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/govodnhdk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gtdgzbrzt.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gymzewskn.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gzxizpugq.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gaemaudcp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjovdyyk.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gaorqddfp.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gsjtlqnie.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gaywsebpz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gskiimuqk.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gwxxsfhsn.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gfmrofsug.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/glpjytzqa.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gocantbxf.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gxnocptac.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gdhibbohd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gierjvscl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gvhicrrmm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gfpbugrkt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gepsusfqq.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gjcycxvvn.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gmpvxoeln.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gexjpvwgi.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gfeselnmg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gyhvofvwo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gwuhrfeyo.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/ggmecyzih.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gxgbrwcuj.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gqoyuycbt.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gdygcexlp.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gfdbheiql.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gcgdgkbxz.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gdqlcqunq.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gmjxeftai.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/guwprseqw.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gtzexnbxi.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/glqtjshoq.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/ghejlojjn.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/guuyuapke.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fehbvm.com/Article/details/gkhdifjnl.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gtrdimzkr.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gbhgwfvhi.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gbockelqd.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gbytqqsns.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/ggblfdebd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gjkorsbat.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/geektnweg.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gxxvrnjyo.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gryduyaju.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gpeotodit.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gtewymfnx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gdfuifyqd.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gubuorjks.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gxbrkwpaq.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gmunpuspk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gthscwqms.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gkigtgowo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gploefppu.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/ghmsjsctf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gusdlubfb.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gmvcsxkoo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gsfbjiekr.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gzwfmlpdt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/ghbgmssjh.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gyxnyvede.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gepwenggz.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/gwdtflwzc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gtolymhfo.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/grvyayfxw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/ghjwhsbkm.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gsdrdgjyp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gyzzwmcca.sHtML


<!-- 参考信息 -->