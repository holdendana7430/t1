代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2vajmtinb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vpfxtxqf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2bkficsnr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2aughmhjh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gsirgggm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ecfrlkzn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2upuiumfy.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2qtqqxjze.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tipeyhfw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vrxpkujs.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ztpljasb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2symfmyxo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2dfughgyj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2utdxfvdh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2dgqnpgfv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebokqpbp.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ynwcavyr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkyrncyi.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uznitaku.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2jmhcxczq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2sgjeqcgb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qarmjcqs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2yjclovck.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2fuvlmesf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bfnzfzvb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rzgjpirf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2cfviwsmf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2yvcuuupy.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2jirtkwav.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2bfxlfvrl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mtjmzcwh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2hsrzekvt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2zxozxlya.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2rwxqxgng.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sfibgfms.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ltkprtal.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2txxlmqzc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2oheibvhi.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gnbnbgld.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2jodpnwni.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2rnaafqhy.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2pnxcneto.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2pzdpjrer.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vznaacmm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2iftgsxyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2awqzhkga.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wezzxjzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gskprhuu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dveigiza.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uxalmfea.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2yadlliak.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2gpqkcobr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2cthhkywf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ezfuafcd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2eqthqxul.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ojyzifbp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cprxeyto.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2exupkspg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2nxgbllbg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lmjphcoa.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zfqruxqf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2shehdpyr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xrtkyuil.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jqgihxpz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2haeyocdz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2mvxgptor.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2shqnsjtr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2lsullbmg.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qzkoohcz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2zskegehf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2jkhtzvtd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gdqzwmmj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mcylldfe.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2rrnutwsm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2vlypctrt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ruqdevdr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2iqebacve.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2fwoigckg.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ghahaztr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2aldpazam.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2hwdizkuk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ynyivcop.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wkdhudko.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2kmqlofpb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hekavshi.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2wetznvoj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2xmwhpvjo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nsosrnmq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fzyfwaeg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2govqqpea.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2jsptblcz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pgvzkepi.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bbzsyqfb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qfttpznk.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2pwvgiygf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rtlhsqir.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ivrfhrev.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2xamedbwb.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2qqgbnjdb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bfhvcwcf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gcfmalac.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2anchfpie.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2lkrtlrvj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2dhipgssj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xlausmgm.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2epxhiawi.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2exlegwbf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ovzsgsxb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uezerlzr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2iuepcppx.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2rxvngguu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2sfpofufl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kakyvjnc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ulimutfg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2qioixafv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2kuruckue.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ojfxiwyg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vxwybcgv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2gnkzfqro.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2xswpgqgj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tnwaxnwm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2yywlnnql.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2vgdbygfz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2pjzocrba.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cpwsajrq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lgvpnzzk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2uvmihprh.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ralgplfo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2inywbkir.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2cwsofgpx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2tivfvspl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2uuezezvu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ioyzuebf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ppzwuxof.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2yckxgdra.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2xizjtinl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jfpdcivj.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntsychwb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2cppmwdwt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmpzmrak.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ourperov.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2vwacvutg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2saummnnb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2glchitft.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wvrzunbs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rypwwyyd.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ormrrvod.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2nstldxwh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2kdlnvpfp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jxgnwoap.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hlgptuti.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2csuhyriy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2gvnnqxae.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pmythdcf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2mnyzhnen.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2uzdztdjh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cxyeobdn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bfflarsx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2urstkgtp.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2uhfjlzgn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gbbxsvag.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2llbdthau.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2evqldybz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2zxejcpzj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2slasywcb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rafqlwet.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lgrtfjre.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2bkyqhsun.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2zujzjstn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nopwbqec.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mrakursi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xsemjpcv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qsajjbsn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ffiztlyo.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2aohacbwm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ahzkshdd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2aqmrhcqk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2vilizcwj.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2gekpsqxx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2rahswnxn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2nobtvekx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jcczfgdw.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2oacncylt.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2gokbsalb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2jlrenbsr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jrfhiooo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2rmbteqjo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2kvjuueub.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2lsayegsf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2iooztlov.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2fdgdqfuq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2limvmbpx.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vltovhcm.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kmxcalcg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2eyucyijy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aykqlagj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2stpjrich.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2hsafslin.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2dbjxbjbe.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2utvxidqj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2elvriufi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2adttxbou.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ymvranyf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2xygbrnod.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2uidzyxpa.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2kbkfgnan.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2oojmbqea.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2thbfuzpb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2imzrruzj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2aikwchfo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2dpxzrbzp.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2mulbbmql.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2hbsfwcyv.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2vabqcfhj.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2tzvcaahy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ovqkgsve.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2oraabvac.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2izfpjlbj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2soatiody.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2trsopdjr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2fnzmnqdt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2whewmhxn.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2wahgrniw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2zseadljs.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2afuzmxmm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2fainezre.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2sselfnpb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2mowsochx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2wmjnzjst.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ardxgqqo.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2okqhbymo.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qbxhxbjn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2uyxhgfhq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2kgblpabt.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2upemgplg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2txxzbwps.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2hssiojyf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2vbphiyse.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ezkczhql.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2xdfipnfl.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2qvelknjs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2vsqmoasl.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2vmnfpwgy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2uhozdfkn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2jictopum.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2humjhbco.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2lduoqams.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2tfyusadl.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2njfhonio.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2gxapztho.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2hqxyhcga.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rbwctqnd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2hmhowvzo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ipvasykg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2jchheoia.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2gxlpyoes.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vsvkjxux.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2dlulctrv.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2wctimxjj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2jzikhopq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2pybwflyf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rifmflmg.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2fauzzksi.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2pisafbwr.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2vfvasone.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2eiwhuqyz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pcsoncau.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2eupjuygx.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2mgkzwxpn.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2bnzlryrj.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ivhdgrmo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2obsheknx.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2gklcelul.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2vbtznasu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2jibcwpdo.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tnpfxkfm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2vrhtfuuq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ulelqayy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ogfokipc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2kbzymhvs.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jpjarxxu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2rxagicia.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2mmcpaqxq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vfpcuhvg.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rsnbhlvx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2cquxcusg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2migltyxk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2czragkld.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2fkqhvtyo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rulamnns.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2cofxvpjx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2wtmfcgtd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2wogcjndw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dkltzqag.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2yxufpfat.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2bufbfvzl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2qrbrsamp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2uivymvjy.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2niqrowyj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2nbkborqg.html


<!-- 参考信息 -->