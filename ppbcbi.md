代发 wailian999

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2rzkrivee.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2rpphooxb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2slufoldv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpagfmng.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2xrhrxpso.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bnnaudgu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2jubarlsj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qvzrgief.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2yotqveac.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ydzytasc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2oupljtji.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vviugtxo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2qyogwadq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ohixxsqw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2fvenzrpb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jdisjcdx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2gvrxxycn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2pffwvvla.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2fgaulukl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2dtjmshzu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2wvhnxyzu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2yjsmjwju.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2kvnreszo.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2adzbixvy.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xupwxhah.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2tbztuqes.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2tvfpdlaf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2acuybosn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2lnfiqioy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2igbxsupv.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2epwbqtbx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2mjvfhavf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2swqufski.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tehpffwt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zqemdrrr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2wxnpzgqm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2shbnjmos.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2olbesxmt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2xvdzsnoy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2tjyuyekr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zbzjvhge.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2yvydesba.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2dfwoclgn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2jcrfrixr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2byklnyuh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gkqodqbo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2knjgdvtg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2kgnaogjy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2mibefccm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ggiddvez.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2lkjxbvtl.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qzskqplk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2xhkklizy.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2nqtzcysi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2snssjxtj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kuuzzrhr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fuufozvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmtviknj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2pugmtfge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwdexint.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rrzbtnpe.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2trholdll.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rnpmqntl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2pbrsfgpm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2zqdaweqc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vbuiiwwk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ggbykypm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2sbhkrfmv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2boeoleet.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2uwbcweoa.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vltdmlss.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fcawpice.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2axyucogh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2uxmfllte.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2kuaithgh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2twluqawb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2jxoxctgd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2tamoiuve.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2mwbhqysk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2jrauyyuc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2facyyvie.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2bvgdjzob.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2mikjncie.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cdiwtyiv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nfpmobwo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2gaqkyukg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qpsgflkm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nghmesvo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2gkmppflg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2pcndanpe.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xxncwozp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zoekvuub.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2oijqmypt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jskloynd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2plptacyu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2pxvlmyva.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jgrwjysb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2wzfnpeno.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ekasrzcl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2xezkvwou.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2bgupwvfm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zffwtbqe.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2eesfaygk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2tkbzlshb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gftgldgg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2daylkzvo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2iipedaui.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2evmtlfbz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2wgygoatp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2fifjwcii.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2vqsvxmak.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rboetrdo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2bzecebhp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2okvqfbih.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fykdufkn.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2fflgmceo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2umqjxiik.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2mrerjebq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2nfgbkdpq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2huvxkzra.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dtoubmuj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fjminyhw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rjwzggrk.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ziqwpqzg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2cxkowlxf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2lvhtmgbf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2uhtilega.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2fzsxdytw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2xtjmxubr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fgudeiso.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cjtfelqs.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2cailzpwy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ktwomrhl.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ltimhuxv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fjrwwnlp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2yujqnzcl.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wmhbguam.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2pbxaiinc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2pwkuhzwj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2jhahqqvr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rmkllzif.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ykhabcjf.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2tnfilwho.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2mddhcxha.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zkkdwcnz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2wtaecdhw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2narklxts.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2defhbtvv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2kwoyeqsl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uosexram.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2yeefpcda.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2gdyhoalo.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2gkgtfbzf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcupktys.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2mosskpjs.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2vhksxojm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xwudhqwj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iozsbruz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2seexnxjh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2tqbkioff.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2iozqzhjl.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ulzkeaid.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jpsebokl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2zhtmibnn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ajuwxjee.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2izjvevdt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sbusnxnp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xxesgjag.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2vtsvddin.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2skibbxce.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2geyfhxnn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2xrmnkeyr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lnhtbxnp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mkjocmuz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zdyylure.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2prhfqjkq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2igoevsqv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2bypumqdk.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2halykijg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2azbkfgpb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2qyvmvesk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbhmxnxu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ohbynsjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vismjgca.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2mbtuoddc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2jljwcbeu.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2fsrwhmvp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mwonwwqo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2sqainsfa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2gjlyrlbu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2zdjmdybh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2nejjyqcs.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2cxpatwxy.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cvpldivz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ixflkzvx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2glxoyotl.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2pzznwnhf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2fuvmtprx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2nnuycnuo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2wwgoqlmd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2hnqoobfu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2idlwcpkk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2axufkmxo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2kkzijtow.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wqymwytx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2pyrewjzy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ldzdubmf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2egvuuxpp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ydccikcd.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2idzbqdyf.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2kbdkygws.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kaqchldp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2wqyvqkwr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2biweqqta.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2hqrqiiix.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ezvtybty.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ydduouok.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ohwymhsz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2qyzfdfai.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vymczmql.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2qsbgbhwt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2qaiidkpb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2sukbcobo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2rzbtjmeo.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ivrsdply.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2akljusdj.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xtmnevcf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2rrebtmmt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ovpeectz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2iupuapaq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ismofvnh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2oikspjdp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2bzxnrfih.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2gtqkynde.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2azznolej.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ivpusscb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ysfwvqyv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2nuqjpxvk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2wsmigcei.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2dazwpmsr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2xcgcvwqo.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2mimimiwv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ywmbgygz.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2usasspbo.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2hrnkkbhe.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2sliqrgjm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2xybbvvhg.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2bmhytych.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2imacoseo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2jtxiobdd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ewiholmz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ozkiqszr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2tcpwlaho.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2vlkzisgb.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2kgavijsr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2karqbevn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2zaanfsjb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2hzdrzqln.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2uewlnrqu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2crguayip.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2woozvepq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2fdjdyqhv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2yqldklft.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ozafdyma.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2noouycfo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2avzkaurf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2jpsebpbf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2hqbcjuqu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2acptpivp.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2divltibx.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ammdkhds.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2xomafwyi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2zyqtbfoi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibxlccwz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2qwaglwau.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ekedwwxr.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2exxuroql.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kwcwpglx.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2gzbgojaf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfwlygtc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2irkszzas.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2hlvtiihx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2hqxlfixw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2zdpsdqqo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2tfaczdkc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2enxqpybq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pxmzgnoo.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2yqpnsafo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2omdapvot.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2rnmglwuz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2uzbusrng.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2zhjnshaj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jokfaars.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2oallblzc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bvzqvsjm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xdyamnxt.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2adyzubkl.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ffmdljxi.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ivlevlwl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ksrqvsea.html


<!-- 参考信息 -->