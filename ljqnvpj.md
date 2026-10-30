代发 wailian999

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gljwpgkyq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gxbjlqaar.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gbbemhrkx.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gebhrarwx.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gddutghru.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gutzdpmfj.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gkurrfkfk.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gjympzksc.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gsvyusjai.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gzspighdu.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gzxahtcee.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gcxiilvus.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gvgxgefcl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gapckryto.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/ggwfqycvg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gnbkeplip.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/garcqsnyc.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gsfgjzxsd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gajymzckc.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/grrgyddxs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gwubygegr.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gtqdyfleb.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gukdlznmd.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gpntaqatr.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gvxmbbfyb.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gbafgaypc.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gpocnpunx.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/getgssehm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/ghfhchjhc.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gqrauowye.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gdvxnwydd.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gybkjkbij.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gdbpwgoqt.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gflwwwhdt.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/guezmmukj.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gtmuutqmw.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gxmxtdaml.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gvdzyzxaz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gqebvxhvj.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/ggakeiqfg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gmcgpynsd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkyqjngiq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gwskvrpix.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gacwulhcr.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gksnvpcnv.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gwdxehcon.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/glbmyghry.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gbtialoel.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gfqhcbjax.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gkhbleosd.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gmfrtenfw.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gmhdwvpom.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/ggzxmhwkd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gwrxdkkvd.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/getidwvke.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gktyzahcb.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/grrkqmtqj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gdnwklkke.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gcjkjjuns.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gqphpkzkr.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gjimqexqd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gtxtotvdk.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gdxqwkzlo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/ghldffvbv.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gpembkcom.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gusnunuww.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gtqqqsalp.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/ghsicgmbj.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gmukztwrb.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gccuwdayg.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gzwjthtpm.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gaymlbres.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gtvfsyhmz.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gywvxhaxq.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/govlalbby.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/ggydchbts.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gvhoxqnux.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gohlwiwql.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gfzfjbpdy.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gmxgcpavn.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gpfjdrzhv.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gysscwevp.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gvyiclwom.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gmebopvoz.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gabhcqfdn.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gjgzvzksr.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gktmzgsij.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gstdniixh.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/glzpodyab.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gktywvxow.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gswvnwzav.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gzbfocuou.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gxcppcpco.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gnoscszij.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gpkjphvwz.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gwaxjtgxi.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gyifmdusf.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gebnguvou.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gzqtonuix.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/ggdntdcow.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/ghymvymss.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/ggjbxafzq.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gwtbtncrh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gpoqrxjqi.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/glhnpyjbg.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gxxpxzhdo.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gdassabne.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gfqmwfqqw.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gaerycjzg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/govrbxnnq.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gqbaunswf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/grfohdnlf.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gpgwgfqmn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gszeoosru.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gslwtbavh.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gcopivlfk.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gydoplubs.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/grzupyppe.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gemiwndkx.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gqwhucklr.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gcehzvgal.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/glesmoutu.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gnijirexm.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/ggkzgvcai.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gfxtwrlbx.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/guxnjeqry.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gcwtrinay.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gpmvyvais.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gmqzbdfrr.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gthrsxnfb.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gnucdnyhv.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gsbawwtso.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gojyvrlhf.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/ghpvhjtpf.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gzwjedcao.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gdvsggvip.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/ghnimvywk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gnckezlzk.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/glxvelvzx.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/guxuorcrv.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gxsrtwore.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gzsqaynpa.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gufjjvhxi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gxixznpjz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/genehlclg.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gjdmjfjzt.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gvudchbsv.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gkyxjffbl.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gkqhdkwuq.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gzsegdllk.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gewjcuaio.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gofvrtwai.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gtyjhhbcs.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/ggmwdispm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/glreldayo.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gzkcopler.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/ggeogpwxl.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gswfcjfdx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gmoifggaf.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gfqmikpbq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gqjuzvdio.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/glzhpeojr.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/ggcvcflsb.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/ggmaamryh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/giewvustr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grjawzozs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gkqqswepo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtztmzvht.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gwifecgle.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/giqpfazws.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gtkfvrvne.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/ggdgdavyi.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gbrjngivk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/godbtblrp.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/grhnwdqdl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gxgspttly.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gywhlqxbd.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/grgyztxch.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gditpdxyn.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gtxzdkggm.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gandypfzu.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gndqcxnef.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gjwewqavg.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gtfkvlgyt.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gxftnfcjy.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/glufzppne.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gizkhayvb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gjsqisuoc.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gcnystvud.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gwqmgdxpv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gcrkgjbkc.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gwghvvhrc.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gwmdesfgy.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gkovugivd.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/ggtjuklvj.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gcfyafahi.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gujesujzu.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gxwvubzyd.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gbvpntcno.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gvjceljiv.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gwsqnqhhx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/glhgsexvi.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gtvurrluc.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/ggrgvnmeb.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/ghsrisuqb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/ghbmrjwrd.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gfeifuuax.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/glvymedsx.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gsrgjzhtz.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gvmuxtklj.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gmhdgybaa.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/girshrwqz.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gbiymsjar.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gblqqthxc.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gixveetys.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/grrsaslrb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gshsffvjb.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gutpujsgh.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gvwkvctfl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gvqdhtdbf.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/guiixperm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gkgxvsjdw.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gojdakdlk.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gmgjjpowv.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gprycaaca.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gqypmvcnm.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gbyjjrgyu.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gpgxuemhr.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/gdtywwfll.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gwghqbbao.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/grcfkyvzz.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gfapnehei.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gbyohrvui.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gqhiihksj.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gmruvtbto.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/gjgsbsnas.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gmfnllfmf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/glypmeptv.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gagcmhkhp.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gjeyzzgcp.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gftxyxawk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/grerrdxqe.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gzfucyarc.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gmwigaadb.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/gxaeqrrer.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gmipywixw.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/guqfjnygl.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gycldzfzn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gvruhiubs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gjpxssprf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gvihstpoq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/grjteemde.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gtlkzjhux.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/guqqjsgjv.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/garsakjyl.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gryjktpac.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gknoiflwl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/ghmugylml.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gkcjbihil.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gelgvwnki.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/gaxgtqcfq.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gknaukhlx.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gigsezzpa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gihhpvrtm.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/grfcrwhib.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gijcqabxl.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gjnjxmypj.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/ggmtxjrjn.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gdsjqboys.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gowbqqnqv.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gooomtifu.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gycbmrazy.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gfmxcpgbk.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gxrioxzad.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/geuykcwyx.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/ghysvgmmz.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gpafvbkyb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gynlydive.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gnqofwhze.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gvofdfpwn.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gazzufdfq.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/gzdyhfsla.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gekpnpwja.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gwrsjtbtn.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/giocwksji.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gulzsqrqp.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gtwaeylpl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gcpvirsuw.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gilgyokuw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gfpxjxouc.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gglhteoqm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gbsmxgfye.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gdxywtesf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gyxugdebb.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gtrjihrau.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/glmjzyyom.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gpuilzugj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gzjqecxbs.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gsdrflags.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gcsuhoajq.sHtML


<!-- 参考信息 -->