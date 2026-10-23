代发 wailian999

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3wnkphdkn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uocxibbx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3fpntagpt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3sorkbihr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3zaxdfejz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mxwpqmdo.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3brlzuarr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3udkqmzyb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3kahjejke.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3huarnrxt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3pxgeojgm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qwzugcxe.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3zpzwguak.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vppygizx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wuojlpsd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3waygnoyd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3vehefjfr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3zgnltrqo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3qsyetgib.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3uzanjnbi.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ozdyatvl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3lrzzkajb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3srjzleik.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3pahpijlk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3zqjkcwpp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3zggxrlim.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3fhvqtvwx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkpfighs.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hlfuimzv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3tdzjnwer.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fcuzqjvg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3lsjutuea.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3duqyabjq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kqjsxpwm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3bricgise.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3zhnoqaug.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ciibxnmw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3droqzigt.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ijqqaqha.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3qdwimqyu.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajhrxjmc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3btyhhkyd.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3uazrdnjt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3virhlulz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zrdkhllo.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3cxbezjji.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gjmjutbp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3steixelk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3sgcgggfy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3afhonenc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3gcvbqsqv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3urxlgpyg.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tvekvect.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3cftrpzwo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3achnhgjk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3psnfksdq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xmswiagt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xjwywgly.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ewjqisec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nxscbgzt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yoolqqmm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jlokdjen.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ftjrwxhd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3fhoonpfp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3yzegdtvh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3cscvovde.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rravkgjg.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ukapbidq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yhcofylp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3abyounvu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hzckiqnr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vrysfxny.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jmpcwtwn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3clbvxyyl.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3buyjowlr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3awgdlssw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3osvdunsb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ucvfdspe.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3bqeyjxzz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3rnttisqs.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3nivvvpaa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3fiufzxim.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3koffnxud.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yucifihj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3bdwmfjlh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3paggthie.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3xampqqza.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cfabozjn.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3pinbcyts.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3dknlgrpp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aaufgpxu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nxmbdenj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3vjzssigz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3xxswbeeu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rvktbenu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3apuviusx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3myamulac.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3jnlldgil.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ehnrzahp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3biytxoix.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ekmrzjdz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3fjpokeuf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3upoawvvq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3odkhbppl.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3hyxhvpld.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3bsplhrgh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3dfxubetr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jsjdishc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gucdpsgg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3eiaqqdlh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3etxopimg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3eowdbkqy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zrcictmc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3hnwvkmgv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3emtdibtm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3huphiaav.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bhsczskw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3yuigptqq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3slknvniu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ptdwpfuv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3juhwpqqp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tjdtffhh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3jsqwrdwe.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3hcxhdwqf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vpvclcoo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3gliuktha.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3bpjxcywm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3hnncnkvv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3egbcdxpv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rcojajeu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3dsxbikmy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3swohqrkf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ghsdwbup.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3erircqpu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ipwwfwbt.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3bhbilhty.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qfywhekq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3cbsakirn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3rsvibwpk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3higkghoc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lekdteuc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ozlgcpkp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3satyryfl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3txtitceg.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gyxrbaxd.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3uckrcthv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ewoqllkx.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iveauykn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3waahmblm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3krkopvoo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3qibfeuxz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhlrxydi.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3qiropqnf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3cdpsgusr.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3qghqjrgg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3mblfeixc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3rbhlmawa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bksynvnw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3crtalrbb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ciazrfmg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhnmnovr.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rigjblza.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fvvyuexy.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vnpbxqwk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pwsspajk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nomyhevj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tjelmain.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3sqowdfdw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3bglmryyr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nfqtrhhv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zmizgimt.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3qmejlynr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cnxaummv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pnmweejv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ieerdmmk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3kvdqcacf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rcjezhqo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3goukmghg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xdvvhxic.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3kbdewfxt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3mohiinuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ynawpwdo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bvtipajt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wolsabzi.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3qovxeikx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3nrnqqlfr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3epxvnxal.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ynlpitgf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3kqqwypdb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3wsadtsgx.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3hfsnlsxi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3hqisczjz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3wglhlupx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rwsabpgt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3fbwsqaxa.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3izmczgjx.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3hcsmnsmr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3vyefszpd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3fvhursgt.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3lkcwhmdd.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3uhodjcir.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3boqeocjt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3dulwvenw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3gwyssubq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ibsfgsky.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yauupibk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3blcytlss.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rzsdsuep.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3oiznocip.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fkzcjdce.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3jxmnciss.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mmaovavu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ahljxpuq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3phlmjvpw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3yhksualf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3vuljcjww.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3zvlgoyyj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3yainzrkc.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3lamslluj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bggpkear.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3dfuujrdm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3cyybjhwh.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3cqzbhdde.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3kasmdaae.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3knwjzspp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3tsudrneg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3txassjht.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3dxosdloj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3rtytiied.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3rveueugy.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3yecgzshe.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uwmppuag.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3inqsctsv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3bsquvoah.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3fuosaleu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3tzavsesm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3dctaibeg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3kzkoqvma.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3elxtoyge.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3iayotttz.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3flchwmlw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3vdpspoyu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mqcestth.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3noekkczu.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3wjnddfih.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3snshuzrj.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3jqajiqey.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3afxbflic.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ouabxsre.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3iffhqsyy.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3fozvjyjz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3bkvahbnm.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3wzyfhonv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3hfscexay.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3wwrlyfum.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3kbllvpqy.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3qzpfekpn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ilsizifa.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3xpwmlaai.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3evrnsfxt.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3rdifgeql.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ltlaswoc.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3wdfdvsuc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3rdbxffzo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3tqhehdkh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3unbmgeia.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3khpivpkl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3donqjrnl.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3pivcbxnm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3dizmjoml.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3irjvptnj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3mcbhczwg.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3rpsavncb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vcepdskg.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3fikhaihg.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3wxciuqbd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3cbnqqdxv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3jntjnokm.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fjvcyzzx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3jtpkhgns.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3xlgybngx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ilrvqhtj.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3rjwbmlnv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3jdvubbbj.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3wnndgxbj.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3cdafixzb.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3cmuogagu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cndmmegm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3xucccmki.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qkvdwmjh.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ixcxzugz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3qzynffkt.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3goeisskq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yutyhegy.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3kwylwktu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zwwhnksv.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pvfzaicg.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3lhxiedkb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3oljbnaxd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xzfsrdpm.html


<!-- 参考信息 -->