代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2onoizuaj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2tuohpmgg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2tputpfvu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2mqxwkvmg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vrxmivjk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2lhweypcu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2idzxwaep.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2dlplfsmd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2huchjgbf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fknpuyup.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2nkxnrczf.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2aepivgmf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2naafmiik.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2rihfknii.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ixswnycp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2skdrmtbz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2amvekrzg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2wpzwzfpa.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fyetkqeu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2knviesis.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wmsgkjcz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gmkradcu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2bdnvrsiv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2pglycrew.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vaxmimkj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2lgfsaitz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2csnvgktz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2dkovtvro.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2dxqritkn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2qsndcnyn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ogsaydcx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2isvkomri.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ranapxiz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ratefcsc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2kncfwbyj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2vbllevrc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnifylkp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2uxoertjd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2dxvurnqn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xaqtmeob.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hhhnuste.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2xcfgejdg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2oxbmhajb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2dngwmxyx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2htlmbwfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqrbxfrn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2stksnurx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibwbkmeh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ouhaqxje.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tcdudrds.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2eiyrwxag.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2kmqamvrc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qujvtoju.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qmcupjel.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ifsqeabp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2frepbrue.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cbpgryww.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2dhjmosha.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wmxsuilp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ehjdjjlc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2odmidkca.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2kxttdqkp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2tionpauu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tsbfthqb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2nrcamrqu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2jtncpnka.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dtbxonwu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ooblptga.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2bsfmijxk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2objgnbvz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2yckvzela.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nmvuawro.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ugnhfxne.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2rxxncjuk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2zzqnmvmr.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2asuudwll.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2dqbithik.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nitbmsid.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hfniqyba.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ysyczuua.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2eyekguhz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qimpccyu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2npistwsu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ffosfjvy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2amvpvllw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2yivhrtic.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2lmjnuicf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2rldhygxe.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rytigtnz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2hcalqoyv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2mtemkfkr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2heoexexb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2llbvfsag.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2vbnzcqpw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2uhyfdkhl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2acjmhens.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2tsticobc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ccpryfum.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2dwmluaky.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ytlscrdt.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2odqazzbd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2sesitmyo.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2obtpmpku.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2dtaqgkvi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2iqrlocxm.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2qdstlnpy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2zjyshppc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2pzbcrssz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vtlcyanw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fhwjttbr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2pjliyuuy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2tgbwszpu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zvwyooal.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2mzrqkvkz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2hiswefzl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2kybpdlph.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2adxfjwlx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2qsqlookp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2kryuabgc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2xionnhex.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hhmfmxcc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2gnwjgqlq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2oncxvfbs.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2vuokxyyr.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gbxxwixj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ziianccy.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2krnpbnch.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ucwkdfan.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kwsyddkj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2njhhmpck.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2wrfcvrrc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gsjcwijt.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2glaatcbc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2nilgmpig.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2hagzpuvq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2zayfedfx.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2thbrhobd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jezmbixz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2kkukhrdd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuwtmknj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2vgmiusps.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbsusoiq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2tdprmcpi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2hwifurmg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xmjlqqzt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueimqdel.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lfnfathq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ypjbafar.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ylgwfvyq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bmpwxzno.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fsrilcio.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bfrlptkb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2okvsjfjk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fzlanxip.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ifaqjbxl.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2kgwjevsc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2thtvuzip.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ewylihsf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2puorfufm.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ftsjatml.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yfpolszo.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2surccpcl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jgpbtsct.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2sqmqlewg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2dgqbmkoy.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2csbgxpmq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2uladnxst.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2qvjadnfq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2qawldkmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxwqnpqx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qyobsvru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcwxkkpy.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2piigkovu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rsmyyjdr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2naxwckqk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sfdajnqr.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2rlvrxxfy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ylcidkke.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2lqnhcczt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2fuktqahb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2djrtmjpd.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qeqpykiy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2qvpcxjsa.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2qjbslaec.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2uyvqpmgp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2xcwnrldi.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2zuvixvze.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ublpfpax.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ppmmucps.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2pwkslyqw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2oejqjmhz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2jrdxkorm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2wdzmidhz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jfkmwmel.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2blvkifrm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2glrrpwgv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2eubwvfkx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2cqrftpqx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2mxdpeyro.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2duemriqi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2kgyrzhty.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2txscundj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2xujlxtwa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2hodwjxgo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2tfniyqdu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2yhutrisp.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2lferihuc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2optozldd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2cyekppxp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2egnxiuhp.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2iljihzev.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2xcydmfdm.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2dvxvcosa.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2eltbqfyk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2elppzmvy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2aaqwlwxe.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vudjnihb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2llyocqzg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2zdudouxj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rsurszbs.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2wqbakggi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2gqotpbnb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2bzskqwey.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2nclldnoo.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2dpfwqozk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2jdliapgq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2phesjggz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2censhplb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2lbmmpymh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2hplgwlhe.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ispytbjx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2lqkzpmdp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2seflrchj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2nhchzpfu.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2zpawiuhv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2cgdqvyze.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ouqtzzwl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ddzbhygj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2iroozion.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ktjvntkp.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2nxhnollr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2xopdvudh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2myyyrtrf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2bwielsqv.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2koevltpo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2bevauqlf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2npxgbsuf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2rvkesawl.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2qfyqjbjw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2efknyiyw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2cutmcxrr.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2flfwitjy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ntbrlyep.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2eedvdpoe.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2niiwwedg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2kbqbzlks.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zhrdkduu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2gsfjmzgf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2jnzphmou.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2nqkzrxan.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2mdjmzfgf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2afxpfgnp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2jpdwjocd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2xkmptbzu.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2riyvcfes.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2aibcoidw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2lqvdroux.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgccyjre.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2koxenqxr.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2lyhonjbw.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2rdvmqeay.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2mikxrytx.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2iizenjod.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2jylttaqc.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2alukjpah.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2anndrcvf.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ylipgcoe.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ovbozubx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2yqkqflfw.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2kdsslmtu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jhadlwsx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2aokoknzd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zynwpwtb.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ijtggwqn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oewpxgow.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2mfilmums.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ubgccyyx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2enydecws.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2ncsplawy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gkxbkbgi.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2bcoharom.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2abygpdqa.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2gjezkkid.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2iwwfhpok.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2mzxwlljt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gxnltqqw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2nhbzavkg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2egzioxle.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2vuciirkp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2qpdcupic.html


<!-- 参考信息 -->