代发 wailian999

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3kfpzsftf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vrfzeuhc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3zdbgarvt.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3kutprpjy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3gugueapd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3eirwmten.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3povhxjkd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3sivoshfx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3tkdypoqa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3oaemyvhl.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3yhoswtup.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3muoqamij.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3liwovtdb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3biubyman.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vqhmcqmv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3tyadxrig.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hrsqkros.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qpblmcrk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tdlfuauq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3rhpcstdw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3stqjmoly.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3byenrggl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3gdkruufw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3haagunrz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3fosyicyt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3irmvodjv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3qonoamqj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3iiilbwvh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3mqzosgoc.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lifhzwsp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3bopypkxz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3xhxzmizm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3xuxhplqg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3wkuvbzje.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3irqkwvmu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hhdfmaaf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3hgtqzbfn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3pywzyhjr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3idyjkizf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3llajovmh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ivntkbtg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fdyjwcdp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3lunwtmma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmxjggel.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ydrkheny.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ksdmklxx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3byvgctzc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3jrhhwsyb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3xzfzpkes.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tpjsrswd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3qzpbjeab.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3grksmlut.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3rjkxpnuw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3lmbrmnta.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mkdknpnx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cfhinblb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vqbhgbvo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cfnnhnht.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3tuibtzdd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rqzflcom.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3smkpjvzl.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3irdtbayv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nnyfiixf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xupphnum.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3hrslbdoz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3cgrxyatq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3zmceyztz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tpooxutj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3sbmhxmlc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hqyovazv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gtwlmdih.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ydybdjrm.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3aexduplw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3tdsvkvvh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qnqjaoko.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gvgmiirf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3eteptbue.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mnucnihu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nifxetsy.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3bvcufbys.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3tovyuwji.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hzifxcoe.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3yrunivaz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pclmglax.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qjojsnms.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ktiegbrg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3drofvsye.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vvmoansv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3unaqsjug.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mchqtfvw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3okjcmxmw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pcpxmbdx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3qiplkkpf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3hvztaege.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3oaftuaeq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ucsvulkg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fozakrly.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3krlevely.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ulnwehss.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3vrpusnhs.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xugweqte.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xshlriix.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ckokdxsj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3rbnjjldt.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3skgpvlzk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tkdbrywe.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xbtiyhsh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qouclbwn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vxzvivla.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3uozjaijs.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fftkfvrz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3esrvnpbv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3twxfzfcc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3xbqszegh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3glmgydjw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3fhwaelwy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jhnvcyei.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3omqiprmn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3uxjygugc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ojhrjplh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ttuvyhvu.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3spxznefw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3tylvxuhd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3elqrngyf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tmnmcgtd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ewhwijep.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vbhtoovu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3hgwdapdu.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fcziwcrv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3feywxokr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3nocxsfkt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3cwbhpcam.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ofrzoclg.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3kqujtjdb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3zerwdtuv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkxlnkgy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3aimhbhii.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3fajrgghg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jvdrchpx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3awqsqwpl.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3wbkvmpdy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsbwaoju.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yzvidnpt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3yiylyafp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibqnxxoj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dmsndmnp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xxggwlkl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kxpqgokb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ebflzqpj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wdqmxikc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tfxnbify.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rpxbqass.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ykjgmanq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hfidvigi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3blamlwmr.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3zfkgfdab.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ldrcoecj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gleyfbij.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3elxasjjf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3xatgpzxt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nilrvfos.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zumyeeen.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3eokrqvja.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3kpyziiaj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3rssywrtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywouswrv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zmysenlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mxbghrtc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3rmtlnrfy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3dwbwaarc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3mgcdtqxv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3cymrrksc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lcoanmil.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3leifgpjw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3utrvweof.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3nxhyzlla.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3uecfpqrp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jxzyzokn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3gtxkzetn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3xszzjkhb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3tshvkvkh.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3skifjuwq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3hhfftpaa.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3pgcdfiww.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3psnvpugf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3rbhrqkah.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3htterejc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3rlmjgxhd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hkvhypyt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3iqfxbdll.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3jwzritxe.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ptlsrmvu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3pwnstmmi.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3lxnietwc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3zwyyxlao.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vqyikhfr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3nnfcsgag.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3alzroaro.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3hcgsfkid.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3pkjxstml.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ogftnjod.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3cnjufnjg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3frsinyjy.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bftfqlfm.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3jnquiatc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3eslcquqr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3avpjymvm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3gxirnvdr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3lpuubigu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3eskfnwye.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3tvwgppid.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3bhmihonp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3hgdnelwc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ynjvlfkp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ytbjypct.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ofsddrnb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3xsrbuayg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3endddyax.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3okbsasxu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3bbrxdfks.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3mshyzoeo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3vjanjxjq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3vvzgquwm.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3dlnmbswn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3emizrwib.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3minbwhob.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3sfcpkwdt.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3exsqbpvc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3vbklslng.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3msispvxj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nrkwiahp.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vewqhkjc.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3lztlxxaa.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3jpvbarve.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3qedyykxe.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3xltrlqkq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3rvxmnclr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3rrgdtmpj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3tmxxjsxc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ghtpophl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3pmpwbrww.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3qcbzqpju.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3hunqnswd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3tpbdwekr.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3vkoxerbs.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3bdwuvchu.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3peszwfsj.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hivrupaz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3sybdqpfb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3uvkoqnuw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3vfdzcean.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3beostpwa.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hymyphwf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3zmeeqryf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3lakzthui.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3keubdkpc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3mvllzduw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wngfqabe.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3dbaioqxb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3lwmbvotc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kajewgvd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3zlvoovfo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3tktgpywk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfxplrzd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3cuohnpyo.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3pnkdxqnb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3nzjkuiad.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3uaihxdqs.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3mkevnzit.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3voepviid.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zyuxwowm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3hrzwpcug.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3trqdphqt.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3btulswxs.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3qzztuanf.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3enxxophm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3depzospd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fotgtxti.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3loemzmqy.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jganpcwx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rjvtaypo.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3dfpjnzrg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ahujepit.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3utekgxin.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3cqxrajns.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nimjxlkx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3afwhmcqt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3uekyumxr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3knwksywl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fcdsnvnj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3cwtwgcfs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3kvcgzatr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3rudlzqcr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3vypnddzg.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3wcaawzvh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ybwewgjw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3pejgbiqy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3psxzocfp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3aiebvfgr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3cxnvcybc.html


<!-- 参考信息 -->