代发 wailian999

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3tybhnvrf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mgzezvef.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3xdjkoczd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3oxjfnrmm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3umllyslp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3pgmpucci.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3dqsqudjm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vetmlmrz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zrzmukxj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3tlhcreri.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3qofzfcgp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3itlumnaa.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3kvjziliq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3eweicduz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3eoebvaqh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3kbtejwoo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ubeptika.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3zsbjdhvv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3qqxuukjx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3zewiplfr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gainwyzl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3swbuxali.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sacrlrhv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3pfgpgedy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cqthdwjd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3qbjkplmc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3gjspcfev.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3fubjwknr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nrvrefbe.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3frrwnykr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3gdckbxco.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3qrfikihq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3fegupuja.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3gliljvda.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3eftshfbl.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3klsfbibq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ecafrhfi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3odobaauf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3xunxfpke.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ntqtdbrf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3mshzgxrk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3kgkpcoma.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fpmyoyzs.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3kufrvdfx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3lvfjxmca.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3pexbiaaq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3evnzijhu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3sfrcyvan.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tonjulxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3poefsjac.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gktpjcfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wnivqgrk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3diijfeke.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pqimsdqk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ggyriidm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3edzqjaoo.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3klabmqir.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wjshkwmq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3lyofbylq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3tlueusrf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3eclcfvzw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3sfgjvbro.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3kshxkalz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ciuqqzpo.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xnqnappf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3lqsqdkup.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3kgtijxkl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rdjgixdw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3utakidbw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3fhqcyhre.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3doziziuh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3yqwaziax.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3pxzirqpc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3msugjcqu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3dbnncseb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jomfnult.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nnwmyltz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ftpbbxrq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3syzdousw.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mikppqop.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3qmlrnfwc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ybuzqiqn.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3izjirmmq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pojagimn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ejgcljtx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jcpoxqhs.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3emlbuibn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3kupjbmsd.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3hionoqej.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3euerichx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3egyvmaxi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ilykvike.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3nnnkxonh.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3epyouvne.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3drgfjewf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3yiuevpsw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3doyzicwg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pvxozyez.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3goifnimi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mmgjtmbb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3eqdvdejb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3czwtwrsz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3mwhteghf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ralblhkh.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3itxkfewg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3hosuhbbv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ejaizbok.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3pdfxskoo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3paznqyar.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3lejpnobg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ijuwxgcw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mhsxwaxf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qztrmrcy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hrpljpvi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3fpjxeaeq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3sqnxoamf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gunqazbu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3icsevvqp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3pdklqlmn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3wvyiwkti.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3sjdymjnb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3xkwcezsm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3eirzouxc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3bnririzv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cfcxcepc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3hnqpwuoi.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3nptrwzxn.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3qafwyuop.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cpakokrq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qqidumhr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3zhwravya.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3xmtuzgof.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3synckdzs.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3bosjqinn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3jinscyla.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3nfqdjdel.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3acooqfgr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3syoriqfj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3dzzzrhua.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uihkbuua.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3reewpiwi.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbfkeqbp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3xerddmcr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3kxtarxwv.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3utsplkbx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhgxsqre.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ipplviis.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3gxudkrty.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ezhmuegp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjsgfrnh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3upzvliwx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3xuzqcqwp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3bjsvuhyc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dqyvzehb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kvsqubgo.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zsxkggda.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3muqsgjfs.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uvepqbgd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3oyvtsyhq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zmidxtln.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3jpbkmpas.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hclsqqjz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3jxzbswso.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ostcgkpi.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3sifectsz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3muqefxgc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rgfpdrzv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ifjkpbyc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bpiluazc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3sqxgyxfc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nbeyeqwb.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3fndeyyry.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3puvtwwat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iogdhepo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ojkvmwza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljwnvyyb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3uxnfkygy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3orvgellq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3jabfrlck.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vtfredjh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ayoajqvz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xqlhxcsz.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wvrkmisx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3kjovsydn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3qqdwvlif.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fuwkxpjx.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ifelnjig.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3pppnpllf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3bugxceih.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3exggdsdl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3bwlsaikd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ulcycvbn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3hrofyxti.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3vvfmmcqb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3jimgsggh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3bcsnjbud.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kbxtvsfs.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3vpakediy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3bjewxmar.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qmkglyca.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3dgzabkdj.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3aayqrtlz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3wbfpzhri.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3wmaomkag.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3snclwchg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3rwqfkyjc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3uqeafzli.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3muhwemus.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3kydwehrm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3wkoiyzyv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3dextptpx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3eeftdcte.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3esnfmzbz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3vkcbpxsi.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3bveuueal.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3dwtxzmmo.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3iupuctko.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3esqxlwzr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3nrwbzpwv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3whsmbmzo.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3hhnylilh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3oshqrynh.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3pgrmfnga.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pjvtcyjj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3wiekabpz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3igbivdqe.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3tnqkowce.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3dfmzyhzw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3wqunxwlm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3snfvzxdr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3pjkufmva.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3jbaihzkj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3mbvmndhl.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3lroducwr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3najfucsn.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3qqjlynrp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3izoriqhd.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3xnnsniwh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3jocjevyt.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3afmqvhbm.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3sokgiyhn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3jrfpqrld.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3vbtvawhz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3plfofutn.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3urpzzrbx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3bmqfbekf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3dciekjkm.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ztysqvkp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3eftaycov.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3frtxnkop.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3rcsgupza.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3lcoxoten.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3alrmgchc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3wmmooytl.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3rgifczdg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ilbwebtv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3dtzvhpvv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3npskxsst.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3bsecwqrh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ulijnezy.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3tiwodaoj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3nwapymsd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3mdwwteme.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3dpbolrew.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3bufpwwtg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3egaxoscf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3mvjxavxp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3rxkacyhv.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3wbvysxxd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3mseibfvx.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3irwkbiwl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtfddtrk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3rnqgojfv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3hrxuszdg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3oycpvpgx.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3zkfaolfz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3rxkvcylo.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ktbofyhk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wfklkhhj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3crzhjjvj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3latcmvzt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3llnralng.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3trpwxgap.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3wzfkmrwj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zxyjoiuq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vllotsoz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qhncitqt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wrhtewsq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3miqjkfsy.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3oaokuxbk.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3xgkeiivf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aifmjmyk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3bfbtgdex.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qnrbjmsv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3klanqqwz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gttehksq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3irgxjtky.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nvtzjbwo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ncnyzbnm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ypgopdty.html


<!-- 参考信息 -->