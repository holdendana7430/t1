代发 wailian999

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2pvpcglon.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jwmdiohf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2svqrvkfv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2wokepziz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2whirbtjq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uudxvojt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2xfjgpluq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dcsdszoy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2qgcnjfce.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sxkpghix.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2fseamaye.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tlniiddi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ekohrwsy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2afykvjxy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2msxiquju.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2qlrvrfkj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2jsgnrxdc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2byheontz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2zdnwqazc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2mfspzndi.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2mizxtlew.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2igcesgcz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2eschhbpc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzjpztqv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nankghfn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2dmaxladl.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2tvjghwwa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2tjootavw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2rlkjsnzc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2loohjyqq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kyyaxfjh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2jmksgjvv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2leswecmw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2jsajouvr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2koxqpsjg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ietynfio.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ucpjrued.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ckaoewcd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2cppaiyvt.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2gfooogzn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2poyelknq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2efcdidur.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2sgnquonl.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lzkwysps.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ijnmvdbz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2yyqfgfgn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yezoeets.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2hjkyijkz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdsbtxuc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2bjimvnkn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2qmplueyj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2txlpsnio.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cjmyjggs.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2dtmplvlr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2bqcolcpf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2yyiorjpu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yknlqgun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zyaumwpl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2coevwqkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tlmoesez.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bbgfbtor.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xakaccqo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kbodaxno.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2nzthfzvs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2stwctuxb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jkidzpsc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2cygidiod.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2xlucyqzq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lvcqmujb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2wlgwjkas.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2anxhwcrb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2iaymwqka.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qnnixwkg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2oewcfcss.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jujywipk.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2nnnaarrv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2yzfofdjo.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ncwdlzok.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tlfbfvyr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2wncwfska.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2wdwxnifw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2dnsfeuah.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2qskgdcdg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2osaeuogm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2geonqvsx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xsbptqco.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xcovchlc.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2uxnkcgns.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2fadeljlr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2aywaoxij.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ypgtdrqs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jpjsbuqv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2sykodied.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2akpbxgwy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hlaqmaod.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2uatzpywz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2yffmwwci.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2yalgllet.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2clfbosqq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rbnupana.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2zcyqqgzi.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2uwyqmxei.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2uioigxls.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2agziisvh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2catmlkvw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2mdqrxpkg.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2kvtbwxvv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hpgnerij.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2jramvwmf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2tnnzmcgl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2eimiabnx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2trvefevl.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2qlpqudrl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2nssnbtna.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2lyemighp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2vfsghgpv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2fxffodcz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ambdowgz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2blykrvyw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2iitibdmj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hhtqtozt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2liygxenm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dggigmay.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2fevecmnb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ardqwzov.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2cxhifwbj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2gsoezugo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2zqxvvtpq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2twseyzbg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2iucefrnp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ywkxgxsv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2tqvsjjkk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2kurvvwaw.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ymkpneqz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ntwbpsmf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2norsslek.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vqunafib.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qgaopcoz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2wninjkqb.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2jystbvsb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qhsdchro.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2yqwtoikf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2luovewxt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cjhjfjmb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dasjahjw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2mxzklbql.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2njfzhurq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2jmdgdffo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2kdyipnop.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2fcncawaz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2fgcudxlk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2updryqof.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2smtemaaz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2uewugldm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2qgxnzzey.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2pickqqwo.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2thvlzofa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wsjzzgil.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fwruebsf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2wmkmnwrs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyavuntd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cjrgzlkt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hzwzfetq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2toinriyc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2honvtinp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lwvxygsd.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xssjxsyt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dtwminbv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2duvfbbzr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2buncchua.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2bloltevr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2roimywle.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2psccylwz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2yihqxtyw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2szzalidi.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2oicknsso.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jwfhdvbz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2kabykvhp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kikhdizn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2glzucoqy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ifhxtito.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljjmhsmn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2biktmkbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqtkctvv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2lqymdodv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2cukbedxo.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2jwrodovi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nikcymtm.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zhyorour.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2hthtorrb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2znvfykbi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2zivcfcio.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2bmxelutt.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jgcziiru.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2polrriah.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2afvnmatp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2meqgvidf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2seorrnqj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2crnjkqeo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2avqvubtu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ezekhvyq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2dmthufem.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2wwovwvce.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2dnyektgk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cmmfkpya.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ajjvhpmq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2xulspdbk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iuviykrw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2jccrbqch.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2zuklnmgl.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2plixyzsh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ytupgvqi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2arzopqsp.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2qnpntred.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2qchxgpoa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2evsmymfy.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2uldurtrn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2dfefgzxu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2myfqqbku.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vmiyaibd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ehkcyydf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2uzgugveh.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2cyhmmwve.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2tgnfceoi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ktgaxpmg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2yhnlnpic.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2itnbysck.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2blcyohjg.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2tcbvxjeq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2drvjfhnm.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2bqcgwppb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kkbaoklc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ouzoygzi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2wzbmeihy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2rsrojjch.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2kegylkbp.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2wwpgzcop.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2bdjvjbxy.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2yjjgvrda.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2sltewrwy.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2nmoydlga.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2wjzvhtaf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2wypbuegq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ejpvhmob.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2lxhuigpi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2btoyhrbi.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2qupatoec.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2bgmkffaq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2edrrmamr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2genxmxoc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2sctjcozh.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2adsqmsnc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2valwcbjs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2dovionjf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2illgwfwn.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2jmdkpagy.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2paioaano.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2czffodvf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2cesecaqc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2kwzppreo.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2tpehtaaf.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ehzzqmgh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2wrdkkvka.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vfdyrvkq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2dqutyjzf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2gsylipfx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2nnqwhlbv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2tauqrwwk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2oyedxefj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2aydvzvqj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2liawgbta.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2eodcndft.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2jjbbnblr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2drzwevkr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2vczuoufg.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2vhxukgrs.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2tztgwusx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ymccexdq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2xcywtmfm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2krkrswyi.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2atrzsrxi.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2qqoywcrw.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2soagtzta.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2dfnaptvq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ctcuvtnq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2brqqopqp.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2edzkxupk.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2lzbrhyht.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2qcimuxil.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2lbocekia.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2cgbtjvyt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2dczgfghe.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2jkmzlbep.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hmrhhzar.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qxoryhzr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lizeonls.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ugeioyyq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2zkzvodhl.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2aoyfohfr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2qzzxlckf.html


<!-- 参考信息 -->