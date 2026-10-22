代发 wailian999

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2qpjuusdf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aviqpnjn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2gsrgaojz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zcgmgzxf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2gxgamhee.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2furckfks.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2hcnalwyd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2quhfdgky.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2uyxchbyt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2zvsvyqzl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2raikurvn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2mizkdovy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2vmivutcl.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ndtvppcx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2bgdardwe.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahosklnp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2tpbczwnv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ngczegyt.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2gtqvuhta.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygblbyav.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ujjbiyod.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2aaoqktfg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jxpxwxym.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2hadzujzo.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2pwiqkqvd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2igtfseez.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gadhpxxv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ldfbrknx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fjvsnwim.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2eqallyve.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2utfxfngm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2iwmnvrbt.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2pvflfqin.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2igdgydbj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2yrntanae.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2fmabrzlp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lsxzodkz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2qccfdfne.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kgcrrdyc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2hygrlnjv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgwgoxii.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2wmwwjhru.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2jhzvkgor.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2yidpxoyo.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2kcbmphyu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2iymqzlwq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2haffqxpe.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ibobwrpy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2arukqefk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2spvkwagd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2nyyftjrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfzxslni.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bgcizswr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zitodovg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2opotrljj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2vrdhrwsp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2bwwdbbaa.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gtibrhzv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ukiygdyf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2jwuvelgk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2hwmrtyfw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2scejulvs.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vzlxnjwa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dvuhttae.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jikshrih.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ahlqtnym.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ngkpksin.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gjhgwcqy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2pbbbtqgb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2gcvtnscl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2waclqpgn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2pymsfpig.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2vmthteou.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nelcgved.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2uqkujfbb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cjullwri.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2xfkiibag.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2eixbiuzo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2simaubml.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pldvwseh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2pjbdcmjd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2xowkdgiu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bmkgvgtj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vivqqjnb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2rjjfaxcc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qmymkeco.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qgmweczz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2odkapkec.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nelvgxic.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2woxtgofa.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2fogdbfjm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2sitxphdh.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2vmduqyys.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2aqsxwsvv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2jvsqovki.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ersdvoro.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ujuzhqce.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bogwtzwz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2duciymng.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2chldbukz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ifkkacgu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xwhobrud.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2mxqvzwqy.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mstlthvn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2njuvrxtp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2teitgvmb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pxjjvjaj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ygrifkwz.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tcelwuuk.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2xnmlyhur.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2dzfscrya.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2bmhqmymy.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xwchlsjj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2siwlcbar.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wemedjip.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2sweuovga.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2frqalchm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2bdgdkpmq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ivivtexa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2qwtjnokf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2wezlzuyd.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2plwxyagx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xmnzfhyk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2tjwgtked.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2blyxbgxh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ufzdgsth.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vfqxhwmu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2loxelujz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wbiqalqw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2mapoznmr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2wccklnke.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2yrwtwyhk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lpjqzvce.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2xvbwdjih.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ihyzuzdy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2kwvvxjzg.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jkqjwycp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2uduhzdac.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xkhdwtvb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2azgrjipz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2myzzvltk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2hjftqrmp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ncbgtans.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ilgubypi.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2bgdworow.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2gagjsiog.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2pyusqdvq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2qkmucjfy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2sbtztxux.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wbczwany.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tdygugma.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2wzlnapcm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2oozfxrkq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2appqjcml.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uklrqvih.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2uprqudza.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qprglgso.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pavpehnw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2atkfglrd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2oglgwspx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2tsnbdvnd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eppgsshs.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qmdqnuow.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2gorgwwja.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ajvlgnlw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uiyikjfo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jiqkvjgj.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2whyxsnuo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2bhdupzbz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2rvtjjfiy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ztjdvwwx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2wyzbgtza.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2kqdjzcpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jrmqbynm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lywleuzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eeaahwbp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2cifmkfjo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2gyerwnlg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2wpwsicyu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ceceloxh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2azwhrnxo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2nsxmrabb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2catgszmd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2kxgwwdzb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2cptdkyao.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qcwyacwr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2hticgwao.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2wonykstv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2zqqdckol.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ngzuvhdc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2peaaklgc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2pyunapuu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ohjbysfu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2fivwtzyj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2vwbnnitv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2jcvqjncp.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ytgaozkk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2llyghgty.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ifuhcxyi.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uvpfcogc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2nuheikfs.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ekbrbfhf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2xpqqolop.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2crrbolzp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2dbtyzmbd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2mhpqendn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2huyoklmp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2kcdvgxra.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2idmbezlt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2xaohxaoz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vhmdhpwg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jmzdknka.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2xtncxufu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ativjibd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2zxwgldtj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ekhcbesc.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2qhznnfad.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2iykxelor.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2oyjcxcbb.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2hklmkasx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2hxunvqdo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2xdfemboq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2yjvxscji.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qdlzuybs.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2wfkjhqju.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2dkgdevtq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2oboiwicv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2thlgbzqs.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2thfvqghk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2lldzettk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2yvrdvsqb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2whuogpym.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ckvjiabb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2fyyrclfv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2slswxegj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ybzjcklj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ozvgwntn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2bfaorgoi.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kpaanbqj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2naajydds.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2sdeanmdv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2wmlphaec.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2frmjweca.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2yqzkucyd.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2detgruhu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2qftphwhp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jitozlqs.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2npnnbhyn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2zkfavwdz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2yrpqxuaf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2nfrymyci.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2xjfjyhuo.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2qldidzsy.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2lrxkrtox.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2rfpcyhms.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wdrsxcjp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2grdndwsq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2xnkukcmi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2rrmcfaxn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2hvnlnszi.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2gszppbvx.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2nvtvigqh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2lylbrqxv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2wdtrkmsj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2lfbosnlj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2iichpjes.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2brvnckrs.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2vbgoajmy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2kjcyljez.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2zdjtgowi.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kpkbrrop.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2prqvoild.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2azaauegy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2igvnlhnv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2uemuxycy.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2kttrpudp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2gfcwfblh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2wfsujuei.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qaymsksl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2znfbcsoc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ejqtcyev.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ybapeysx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2cwzwdpmo.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2idgycxpm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tlcbjwxw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ipadoigv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ksxfdldo.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kynswpmr.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yyhvxjmj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2olhapowh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ivhxjqfv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2dhsecsor.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2hizrqglj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2sroiqesk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2bbfbfnof.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2zhtoenoo.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2mnfmsspz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2uuxgpqwg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2bctmbkwt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2hmlyidpg.html


<!-- 参考信息 -->