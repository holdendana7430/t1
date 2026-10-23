代发 wailian999

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3lrdisytn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3vetwmmax.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3lsrpuoqf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rdklfard.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3qkgkyjid.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3dujaugst.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3abyjotuh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3tczxjohd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xkyceevl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3envhogmf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3blmizisd.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3swgohsra.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ebrhkwcl.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3udtxgbgh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3hnctwplc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkxypbvs.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3fwgjyacl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3iszzqycs.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3phxmjitz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjexgrxu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dqfincln.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3vgzflzaj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tywqeepy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ckmjfcux.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hzxfvcmd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ihxfmhfe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zuevgosw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3abzwfmup.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tvycxkfr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3mdhkqddf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3dhqjqqzf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3wonasjbx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3togsvpwe.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3jpbivbnv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3oadoddlh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gyidpbfr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3nddikaaj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3szbqkgpb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3myaaqzcf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3filxemrv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3utrikfwn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3tevmkiwe.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3otynmpxe.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3rvutiiyy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gypttgad.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3pmvyuysw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3lahxvpqt.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3zvhmtwcd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gcfrjmzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixexqbog.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3fgjdmftt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmavaqlx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tdwxotmk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dddurwpd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3uvxlazrb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3imgmizow.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3staimpld.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3omrsgokw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3jmwjupzu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3qoiphgfu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gptqmesb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3faotlqsw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3framrdpe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kvgvmvzn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yttewmae.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kuallsje.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3zdzxtypg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fmqmmrya.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3opzhtveb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3rqbedhfb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3qpelzmvy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3kjewuuzj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3umqejynv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3dqliekyd.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3cneanwny.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pyrxcpmj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nuyhzrdq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3vytgaywz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pevfssol.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pivcotww.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3iyykqvan.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qgjvgcrb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zcnrxtjd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zudwhlny.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3fqlijrcr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3hgfknzrl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3osmueyrj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3rsotdizw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3maxhxapc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3xhjushyt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3neaxusvc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ogdlyizf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3coelvjlx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3kqhfhakq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3xhwuoyeh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jbyuaitc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lcdlaxmd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qqanipsx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3sivtkpgf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tzmgbpwu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3jacwuqfw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3qbcqjdxw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3iywdfonz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pmfmcgov.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ymyjfpzl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3wybqlucq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3lefoghjf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xybstsxo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ndktwhqb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3hlmwlimp.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3gcepdpqx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qqebyohk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dpobytig.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oflgcpms.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3nvitrrrj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zxivojfp.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3jgwzadec.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3godwefmh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3tvsnxnoc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3hzhazsdx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ksujylsc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3bfczcwaf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3kqchclls.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3faywtauj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3iexcaclu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3motdfvjv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gipryhzd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3thxvjgsz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3myklntvh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3cyxzwoos.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3bklugmmj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3uebhzchl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xgpgmxbi.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3eswsatvl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3gszbqvnz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3bugxttyy.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pwnitpkh.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3fryplesk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3szqknvrr.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3sbmuamsu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cvhjqsqu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3qnrmliuu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3tvrcmhwc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3smxuooer.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3etelratx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzgxhbuw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zvynuyrk.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3tiyqjziu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lnpalrwz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vjnuuudl.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3utajqdyk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3busggqsl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlxnyxrh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hgfvxfwx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xjedrjux.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xsmmrssi.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ptkaxcxm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dduidmts.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tubneqff.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qgtkjgpl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3tjfpsgnh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3csxsrrfs.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3khntalfy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3jqjljexp.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3goycsovj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mxdfxyht.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ertpfjix.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3vuwkejfu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qkhrdcwr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3shpltcba.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bdnetvhq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3zuwtdkwa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3pjsadxzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exrxzyyy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ebscjbfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qjubgszi.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ssgsilsk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3yumgsgnv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3cxndgnno.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3hllvqpcz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3cqnzyerf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3uqhwvwcc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3heghuapt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3uyzjjyee.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3akfzzipr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ukjyppwa.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3jdbqhonl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3dvmmiwem.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3lahpvuhb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3fmfpcjwe.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3kstfqjxw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3rimxlhzs.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3zlwixsgu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3suulnbnp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ahnynokp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3fvyvizln.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3navwhtvq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3abhdmukw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3cutjblnp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jjwjnvxg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3vuejdyxv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3hayhiurc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3eunvuece.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tupssdae.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3whozonwn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3xjkymnjg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3zufbeanb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3uusftkzm.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3pxbinvos.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ujpurfgq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3fnzvsrhl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gvkczfyg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3slkvwvux.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3wmrtwevp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3kkklqijo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3tntjlbzk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3dqmqbrjf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3pvwrnsnp.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3eliegwll.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3fnndvqou.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3gybgfgwe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3bwkokbjq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ncxwvrvd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kemafekn.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3eajxygva.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ajqsygyr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3akltcumh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3idqvfgiw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3zkakjmxu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3zpllfqko.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3rkhvritd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3qmkzrqvr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3pfzbitde.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3dvveewqt.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yuvjtjlo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3osyiuxup.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3nuggqgyh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3pvorreye.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3cknwhiab.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3xionagpe.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3qojizicw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3xhrjwkuz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3zunynxdy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3wgndjhym.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ptykrxzi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3blkzsebq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3hiapzmun.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3yspymlht.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3rsqxuhtc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3uubwsadx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3wdabsgtx.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ggjgtnoz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3nzfvrfmb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3frhpwagd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3fhrwcfrr.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qqposkye.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3iylbrpvs.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3fnogsmlq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3vtdcnqby.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3upfngtva.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zmdflwgg.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ptcthhca.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3qrdzcrsa.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3decorhqt.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3fetrzknh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dbakqpdv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3vzovlpzw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3fjymqrnq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3wgggylhp.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3clolqonu.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ddamoret.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3fnyilrqo.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3fguoglvt.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3nhxxgrfr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3yxquhnwb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3daryddsf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3wnrkbezr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3pgvguzlf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3yqtsunbm.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3aqvfrnel.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ztdqrcnb.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3efnomlhp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3myfuuuag.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ozxlxxch.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ovjajraf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3inbwtaqe.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3moaqujlq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rywtlqsh.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3weltopcq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3smyfguac.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3xhamvdyk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3drztelvm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3fsbigzye.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ipoyvqex.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3mafagqte.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jhbjolea.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3inedcdte.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3wzifytpd.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3efkrcbva.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3xmuxqpbv.html


<!-- 参考信息 -->