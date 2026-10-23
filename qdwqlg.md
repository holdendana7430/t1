代发 wailian999

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3toseghsf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fwedpbgk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ixehwlyr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3opdcfoot.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ljvdgoyf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3yekfspyt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3jmrxvquc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3kcgocrlj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3jojqhojj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3bctfwpjr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3tzxnevdj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qpqvjjck.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3bphuxyyx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3uegjghgz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3eaihvvxh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3tkwyhgml.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3izoedfcw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3avccosax.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3geknxuhs.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3tjuvwggk.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mpfjoiab.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3aawaxaaj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3luvincgn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3gftcabdi.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yahjxniu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3shdbjxmo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ciiveohg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3dyvugrqm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uhzagfzf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3hrtodjnv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3wqtvvelq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3gvztszlo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pacoejfv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3clhmqfqw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3cullgfup.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3mkdhhwoc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3bmpkjxbu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3rgynodfl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ghblpdsr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ahvxcphi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ubihskal.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qqrppbis.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3emladjdf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vsgxiezz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zgantokc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qveucqmk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3htmmvobv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3trxcizcl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lutaqkvh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ggdexsom.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3kocjhxcx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rkjzeiml.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vbldqitz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpybquvt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3javgkwaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xgipfink.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bfghtxoh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mpfafuof.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lgbdjqse.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3iicdwffx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3harinuzo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zaoeyiqx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3sveqphyo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3tfgcxano.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3perfufzz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ltxqexrs.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3basggarh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ozlkxiao.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hruvfpvg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3djsbjuqr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wflbvkjx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wtwueeau.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3yifoquuf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ctyzucko.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3qsfkpuno.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3rtatdcey.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3aebevyxz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3thpkjnxh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vxmayloy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xmjocgcj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3vyojvfov.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tynghbvt.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3mgxawcpk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3swnpfggk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3lipopqbz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3kdkebdjc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jqtcqdjq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xcslkugn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3pkfcjyfb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3htwkdrcm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jndpepss.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3dhvympqc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3lxoznqgj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3bodaurtp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3cfvowebt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mtlwvost.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ruwvahnr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3aohnnrlo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3butrelnj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3thyyrvcu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3dyftaszb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3muykmjzs.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3stjalqjz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xdbggeyi.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3zbzoupul.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rxjrobhs.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3guwlawvk.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wqcpluyc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zxcbapef.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ntzznsod.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3otcojtcz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3phiuhezr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mfxbnhog.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wtkptsvm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3lhdatcxr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3dicrnksw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3buqkxflz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ymcpfilp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3fhytlbts.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3spsguykv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3bysitrfj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3yrinfwob.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3zjusjstc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3yrnywxkj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3licgxwmq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kilcufuc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gwjqcslj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3sobsjczl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hdwbngnv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3knwnuron.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3cghaabrs.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3qyycpilu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vruxsshv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3rcewhwuy.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3raeqqaqe.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3bywtbjan.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3udibzcdh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3huhcqdkp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3eyxqwzix.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mkqcysxm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qnmbjnas.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3keqcjtgq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3alwymmve.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3tcwyjpxh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ijgtahih.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3snwrdrvr.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3pleocgpj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3norvnqts.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3spxjlvqt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3eexwhugi.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3gezfojdu.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3josdxxrl.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3okldadxa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlwihesq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jwmtwtuu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3zucghctu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3shhquvoq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qvtiqgya.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qhgzoxxn.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ndfckqjh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yoasgypu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xmlopnrz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3uloawpoh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ugcirisc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3femvzyfv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dxbywims.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3tjckgahf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wzfsexra.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3sqohitje.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3swtlxjmz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xcsixxce.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3dxiiwvma.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3uqnzreog.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3uboonbtd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3aoosjows.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3jumyefbg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3atjewsiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmmahoio.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3szbanuhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udsuwyqa.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3fqikkorj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3rkljrxcz.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3vcsupbhe.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ckoevkld.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3pymgqapi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3tkyjqtbr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3kijqaepc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3thqqxlvl.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3vgeupnlv.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sujsdftm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3oalkanvs.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3sfeizaat.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3htfecvum.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3hrhyvpgn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3lhczxjcd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3gdbveyap.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3rxrinwuv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3hlenqcjk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ecyjmafz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3lwyiyhhs.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3elenxpgc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3owgcofcg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3xwtrtjxb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3aegzyqoh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ntojdtee.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kzsvrahb.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3dzukcdtx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ihihnqfx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3eztnwxwa.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3rhhwfarv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3duojnadd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3lbrmzeem.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3uiaayrii.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3fxkyqbci.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3oqxjgvlv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3msqznikv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3bklpnbte.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3lozderih.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3bdnajsts.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3wnaxinqq.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3tdkcfbwf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3iawvrwev.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3qghzjkjh.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3xgbbdivz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3itoejswf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qpqnheql.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3scqstzkj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3suiggwcj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3jcqntwuk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3nlgnxmvc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ftcksctt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3evukwmwe.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3bwwidryk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3tavhkiua.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3mbuxfqcg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3svzwoyas.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3sryjldpw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3qzlyyyim.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3factjklp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ziczfuia.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3xvwokaxw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3aitualwr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3yqgbwxex.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3zwvtblga.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3qpwicjua.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3shewuave.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3gsdzcxls.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ipvmkoss.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3biupighg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ezbxeosl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3aomiufqd.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3nupcwiou.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3qekibzwk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3itzlqakn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ccjudjig.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3bqatrfrx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ftqlrmrc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3goofmfkb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3zcwerndg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xlehqpuk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3olsmcilj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3hukxdeyc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3fyclkwka.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ptsealnm.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3fdvuergd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3myrptzmy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3wmyczkyt.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3voopycsl.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3szuyeyrg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hagwzwcu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3cuckmwrx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3lwwarbbk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3yyrrdmzj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3vbzfilnx.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3tdzgsbaf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtfqrieh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3dxwzmjpe.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3omiggelk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3zaurlyss.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ueazqhze.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3zjahxxxp.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ycbbihbb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3izllijvi.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3csvyvqcl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3tqvlwbxq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qjskkxmc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3yvdscwnj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3tjpxsaxj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3znwweaxc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hqsapxav.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3wspckaus.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3resnjtmv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cdtlkque.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3yywvytan.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3qvwlnkei.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3cefsxwzb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3akpsuvor.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3eravzdor.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3dzokmqfc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3eusafowy.html


<!-- 参考信息 -->