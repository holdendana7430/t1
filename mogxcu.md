代发 wailian999

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3fwskwwgc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3unynrybi.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3pmdcjexb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3yvewiwlv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ekxncqef.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3rjnzikhj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3mknynaix.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tcahqawg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lahdwevq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3vnicwwqz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3dtwrehev.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3zlsfoddc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3jsyrhpnp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3jprlqyyg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ouphpntc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jukkjbfr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ocxodjbh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3swupcuaz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3hbazhpdn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3aiczlxle.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3eetkomur.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3jzqxclxk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3racjeijs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3yvcxknxp.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3buccqgmw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3gixcpire.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rnzhgcya.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3tukbgdsh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xpzxynmw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hvgwpqbx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3evhsfxgl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3wlbsqtds.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3oncdokff.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3abvceznc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3kwylesow.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3nzjwgzin.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3lvjcbhxw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ietgodxb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3byyshycb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ssanixuz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3cvcaomxt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ugggpcwc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3kvcayhpc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xwzmllcd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3urtbxhyd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3htznmpju.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3dcjzgcor.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ejkotbqn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3zmbmbdxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvuswgmv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3hqcgahhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iczsmnxo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zftgzntd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kgdudmsb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ejtzdxfq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3hosziyui.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3dgzvjwex.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dymnykpe.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ardilaiw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3jmzwrkbl.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dmqfwjsw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3fxbdztsn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ndukpkdo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gjdhdvhs.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wapsdkch.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3trgnbdnf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3uktftyon.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gmgzyvdr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3hcjshspm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3aqpomvcd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qjpoyxuf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ayeutcdp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3jqdjlgkw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3snlywdsj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3bztffpmy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tjidtpdh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3usomjdlt.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3yrtfqftu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3vhpbxwif.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3oylqdais.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3xbyzjkyg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3nqyuwlzw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kkccswvm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fnujuugq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3rhkdrirs.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3juvbdywq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3owkugmox.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3xqhrngje.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3laubrjxe.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3vexeigmk.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3bsjwheym.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mbsezrkk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fcrixguv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3vwsemnwf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ulcqgfcn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dpitebfe.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ddhykrdx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rupgorel.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3anunlxzk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ijvdgqcd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3lbehyncl.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3qligwkeu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3toofakoe.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3etpwrnrk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3oqhtiuvm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3dtvlyupy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ljvdbcnp.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ojoycuwd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3cowjyrdb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xlnwdwzv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mxcwwyjq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3pvnyiixy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3scukjwgw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ngifobqm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cmqserue.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xrsbeqvs.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gpklunid.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lxznigey.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3oxrymycg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3vdsphcaf.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3wuajpskn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3fuznyajh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vayoiyzz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3hqzmfpfr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3lgpifxwq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3qsmdjdrn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3qwzhgesm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3suydamor.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wfbjexbp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3sqouknqg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3tnqyioif.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3xdfcickg.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3osibjpoa.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3tdlbwmse.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3mpgyirry.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3widwfrvs.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cyczgevv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3jwvjoiam.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3odbsbotd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3qciyfwnu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3osyvfcrs.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmnbxyuz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3biryqdfq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3lbwrpulg.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3xqvuygij.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3sjpvwcyr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3gyaxcqsm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3jmjbgefe.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3vgphtdly.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vysuwtee.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cfffpdar.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3qxkhskha.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ggetbaga.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3akxmovri.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3iuyhguvz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3fksiqhfx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3iwvtfnvn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nlengeui.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hgttlcnh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gxvyeitt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dmpfeiuc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gsfwiafm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hjujnvxr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3opksirvw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3uhltpxcv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rxnpimhj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jbnaenge.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3rkufuooq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ilscbfcl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pkqdnapd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wqwducqv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ohkqevrl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3qxuzlntc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpwffooc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xyacmmax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wmflfnso.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xupuizad.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ylvvgcve.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3flvcjpdh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ozxmhumo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3xroxkpbl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3zxkktvpn.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3htnbgipk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3brikkxfn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ipallglm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wimwigzs.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3nyuazvxr.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3jfuqaqhc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3dgsedokd.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3hjbdkvdq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3uabtozpc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3uhripvxj.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3gnejazha.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ddszvzae.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3pamosvtl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3bsmzbgoq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ildyfxhn.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nstfpmci.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3gkfkefpw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uvtmjnjo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3gybehgpf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3tpgihqft.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3adxljczc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3invmugnz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3oeuumymn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3htzilene.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3fotmzfnd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3vmnedngr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3rpmpmwci.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3nsdqrreu.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3cotbefow.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3olgxdlhf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3vfhufygv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3irsiifop.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3rykpfyzu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3cawhmtya.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3zjwiadqt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3zdtfafuz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ontlrung.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ddplhegl.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3woecjmce.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3kmxdjjgz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3dpsbciwh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3yfkztdni.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3effyhodt.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ntpsyzju.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ugsehmsn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3qsemdcuw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3jffkfhql.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3yzasecxp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3kgfsqcun.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3oytpgevf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3setywbcd.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3fjxiruoa.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3wcstrqlb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3mekgolyn.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3kpaystle.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3kltqqjia.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3izfmiwbq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3dcbriich.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3pzpnpvhz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3dtmrwfgx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3uggajrfx.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3yskxwhyh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3bcodtjrj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3qtfrnmkr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3rztviknv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3nphyokck.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ojsujnlh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3untzxbfw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3lsgxsovr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3mbjvlqrv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3cimawcgs.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3sifzhaun.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3rwuduger.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mnhhemqb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3hqhikwct.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3hulwyhez.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3nynxbduu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3siufysfb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3walbrgih.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3xhsaalsu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3wzisroyf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3oqzwpgvc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ayrwnxoh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wucvcoza.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3tvtwmmfq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3btnoooil.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3hpujlkis.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3wyonskwq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3xqitfcio.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ybvrqnfr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ccokojdk.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3cxvrvxjb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3orqswsfy.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3obhwfuhb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3znzdlnff.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3pcxqzpqj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xifhmwfj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3uurcnhex.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3hieefuxf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3neiwyavs.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3nqsnzkxd.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3uhwrklgj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lvtqyasq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3lsxkxsja.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ddndqllm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxoxhpus.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yawlrtmw.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ckmurcfx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kvqqmrxq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3xulurlsu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3alkakznn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3iivzhvup.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3uvrblsyq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ihxjwzrs.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3cqvlfffk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qgdmowih.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3funwvojs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3xqyflkxy.html


<!-- 参考信息 -->