代发 wailian999

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3vnihhesj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3zlxtrpwn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3rajvzqfn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3xcqkcikn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3krmkprao.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dtfxlibi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3syhobmsb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqdgphnm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3kahzkjyv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3exfzceit.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3navfihau.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3rzqjlukv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mroyfxtk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxcxvbxn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xaotpokl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rusdkfol.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iozuzxll.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3hmosgbxs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3crezkrgv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3qbvyinek.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3djezffab.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3fnzzvdmn.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3xpvjnwcz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3qaqggfrw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbdqczps.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3cgxuzllt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3iwcrkvue.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3mnubagxh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kztcdvkc.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qupuvhjb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cdhvbutj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3xzunwfiu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvfwlcjd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3jpacyfyt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3qutawfce.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wrkgsxtu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kigntgsf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3hrhrffzz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3qrlriumy.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rgzfugia.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rfdvamgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bsqmxrms.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3vsjohdew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tllippvx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uulqawyj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3irlfxtkx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gwdwujqh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3zyqbxjix.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3wjyjuyqf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pidsxzny.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3mxhnrfnm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ooqutoom.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3urjbssmy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3bkcykoob.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xtwvmrll.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ylbfcmsq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3slmjpifl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yenepvty.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pxjauime.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xvitwsqu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3uxtpduta.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3alsrqoml.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qqnhwkjw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qxwvfkxw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3teuxendt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3qmewnsuh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3yxqcpvhw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dcmpbfyd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3euoajrdu.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3avbfnetl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3witkpsse.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pbqtscyz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ialyzsfw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ogiqowpa.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nqmewtgd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zycxzyuk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ijkzogfl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3vbyyhjgl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gbhlhnao.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3pcrxfxyu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xyvvsqbj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3crrnkeam.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3pmelfycw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3memsjizs.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zkvieqcj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3lklbwxaf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3agjtuquv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hgujedkx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3zqbbubzg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3mahjubnn.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3oteleeex.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tmbyzulp.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3wstokeuq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vcfhskhc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3jgdqysed.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wqoqxyqi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3zonbdthc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3wtpacrte.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3qdmmkghc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ihntprvs.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3vtwxdfrc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3huxncfgi.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3gcaljfpc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jmqygdyi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tapqbpup.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jdipxxal.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3grtyhhks.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3pyhamanu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3thfccrqc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3zkgrddkb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ruvokqim.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3dddyawha.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3qqcycodo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rtaojepv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bzndhzpz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3oxfztghy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ontycplg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3uhrkrssb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ncxvcall.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3apmbmhax.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zralrdkm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3vshtcram.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3hvlgsegv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3bpkabogt.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zttuboaz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3yvhajwzj.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3frypxkhd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3wnojzztt.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vimkqgkj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3fbryktge.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3xnentrhd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3obogxcvw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3pdezvxpl.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3qrgkkepl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3tvrqkogg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3bfinvwvv.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3kdtkcuun.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3fgdaruzy.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3rvbiykqy.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3yrggreck.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3gppymxmp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xqgqqhej.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ihqhynop.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3xtucgwlc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3odebdqcy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xdshrkpv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nlxqffqk.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3copvfwjh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qjxpwwvw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ahjggfee.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rxlupqle.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tvgepcjq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qrhjndyb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yppondbf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gjrnpleg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3smklibcu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ppbdheak.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xpczuvqf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3pscpzzuy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ezbundjt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3rngcivbm.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vtkrvszv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3fyshvhjh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3eawauumn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3cbmxajng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrtwlsqx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pyswkokp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iyjbeahd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3avhneucs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3wyhrqemx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3rfpgtxne.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xjeqhjla.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3gnyguhsv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3aluvxslu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3jkmrdico.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3wjuhpzjl.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3pldodnwp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3uefsbnvi.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3vunqifop.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3atrnrnwt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3mxvevqfw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3mvgrxlzb.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3emiroyjs.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3eqbzhzag.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3vgqrdqpj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3lpabkidx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3kovesirx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3udtuppwx.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pgklgodf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ktbjlaka.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3syigmemz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3enhorajw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3dnzadvue.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3kpwaqjnp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3zwlmerih.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jdokxhkx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3bmnphrjl.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3yyiqqpsq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3dqflqhdg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ycvzbmwq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3qstexdst.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3cejhmfte.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ikwheeln.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fdpshwso.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3hfjxlwfa.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3cazboxvz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3mdzwwnbv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ncfmgrvt.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hsfycjdz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3zoeinheq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3icssednv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3rizhbtmn.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3fqjcpbkw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3jpxqewco.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3osqxxxig.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3anonzeqr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3omwwcghl.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3kfdlyilw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3sqmncmff.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3jsvivpvg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ldyvpsiw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3epbgmssg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3iruxnssf.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3hpceiucr.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3mbjgpvrb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3nypwylvr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3zgnhwugt.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3hmothtdy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3vtscocpo.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3qrfkcxnn.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3mrrgmato.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3rjmwcpsd.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3lkjbzwrc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3whfxztyr.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ryptzhwg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3aflrjyhc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3eqamzyfv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ugybhmrq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3hnzgroow.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3xrbbyuwu.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3sfqqsawu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3fqzleidx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3yjkkqkll.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3cacqqgyz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3oqpwaxpi.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3kbxjtxzz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3xwdvvgis.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xqrizhxk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3kmrdxcqz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ffaoaqbn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3qgujywgv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3gkdjilmm.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nftogepq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3yatqvacb.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3qbsfgjox.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3qogdvkyv.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3qcdfnbbw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3owfhxzmt.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ergkhqfo.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3srzjtash.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ujmhkkrv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3hhvkwgzo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3qtnvrxsj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3egmillqk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3awzauoho.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3yazekkty.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3boeoztiq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3imbwayom.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3nzzpewmo.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3wqxxztam.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jdqytnms.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xneowdus.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3uuhixzdk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3flgkiniw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3flxxlsyw.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3mfwtdyac.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rdfxkkfx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3zcuncjcu.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wrgnsgyk.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qtuzunoo.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ogsablfj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3mrwqrxvb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3tpdcfpwg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gztutsrn.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3huzmbtur.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wggtuhmo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3cazcuaao.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rxpttjtb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3cyyeotiz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bntrbgcv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3caqecwum.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3wykbbpwt.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ptofmaek.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3gjgtmrnv.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gkeoltsd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ovozdozd.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3cognlgkk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gmlunjgo.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3nfldbydc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ddvwskxg.html


<!-- 参考信息 -->