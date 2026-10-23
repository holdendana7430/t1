代发 wailian999

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3hlwbfgzn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3srkrzaur.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ohcdmcjo.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3oexbzrng.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3rwkueqko.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3adddzytw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3njifjtxn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jigzohnm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fpcegyvc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3pthodygg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3gykpuucc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3cgkgspae.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3kwyhtnpr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3noguumet.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3dzxqzvpp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3anyptvja.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ryfmiieg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3mcmeplyt.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3cbwazerc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ytxzqowb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3cgdppcef.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3rplkgnow.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hwmdtsas.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3cbojwzqy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sfgchyyn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ontvvizv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3uwevamar.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3agtaxual.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yirazdak.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3arzhsrne.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3sbnxjwbx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3cmfzztzx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsrhjwcw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3efjmdtrq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3arhilucq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3guchosdy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3sqicebnt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3muwvhtyg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qyiectlr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3kwhutbhj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3egzruoki.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hhxyjrpl.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3gnxaizvk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3iyeupxfk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3xkfwtpdb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3dhlobqpj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ytcspken.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3rdyzknuy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3btdlpwxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oumaqxjw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qgwdnzvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fszmxpmy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nqqjhrjq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vexyifle.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3oelutvkn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3rgdiprjd.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ocnmgxfe.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ypuxeqce.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3mpncfeaf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ktmkuczd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zpbwfqsu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3vcomxoyn.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3iwsjgvkz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3frlagyys.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lpizvqlb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3udvgonhx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3jqixkfft.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ldadrrza.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3xzzqwryb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ogukgxhi.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nxerlbqd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ldeocgmr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3cdvhxltd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3imgzfyck.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3edbpqric.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gcscnxxe.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jsmqmjkj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3dpgctmbq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3vlxuntfo.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qjvckeih.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3peoobwhq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jpcappkt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bivjzaja.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qygfrspe.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3hkeajfmo.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3tdnrchuz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dtccqvaz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3xhyimrfi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3inmmwcsg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ggbaroci.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dxbjxyoe.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fzcqywvx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kuapufxm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3imrrufav.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3gcteybna.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3flnxxedo.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3xswrwfjo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3xrtudkkf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3onlesjup.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3glcewvhg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ivtzgzlq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3pvoanjry.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3lmepklms.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mxrroovi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3zifxvfef.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3tyeinvvl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fbbrkfhf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3iruintps.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3orgnmfrw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3cvkrdmwf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3jwkxklgm.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pnylzwtc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uwygcydh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ovvcdcsy.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zmbozegs.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ggrlkdpn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ebiizoua.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3lfejdfrs.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3syftxblw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xahjaaaz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3yhzbrhct.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rglrhdoy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3khjvmxtg.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3dfpzuyrd.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rwlrepes.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3rktkjkyo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3aovnwqdi.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jixjkmze.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qhvsfsay.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3pkklwydv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3rcaercib.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3aplfukfo.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qazzepvi.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ikkfocyc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jtwbpmor.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3qqjojmuu.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3piehnjji.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3wvsztrvm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3umgawrqr.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ikfepluy.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nlmtjgds.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3boxiiqfp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3dvgwjnut.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqqpzxpt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3kzhxxinz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3zqbrbxjm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3gaxbaaax.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3dzkzjxba.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3xymopejf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sztukbbe.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pupsiysp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3cmdaohsr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyqicmjp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gonespjf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zjoyoums.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3tljetgtn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3amkbtlie.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qntndyly.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3anjunuct.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3eyfajqno.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3utwxaoiv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bgbetlmb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3izrgmdfq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3zaxjfjhw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3dgrgtdvn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hnoytzzi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3cghycynn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3qrzlwpfi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fqxgylko.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fvcgjutz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jmxluhjw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3royjmkcd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ebnfccne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uyiboaub.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3qrjedrow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jehwdljg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3vouihuhv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3qacsoued.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3aplxsbdk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ktqeacpa.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3smcygvff.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3wskutqxe.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3dcugkmci.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3xyqmjnkr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3qvcyvlmf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3izrzfrmd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3poiggrxi.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3geurcxwr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3jjuuyzjk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3krqmqxmi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3xmgeurbw.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3mniffmkt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3yufjotwl.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3jqnxsusp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3kiwkynft.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3syagvrbi.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nuilkcwr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3mfzlilqy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ogpqguvo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3otdjgcrk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3wnfpgkvv.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3hbgnhwlo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3pqnsxttd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ibyzmcor.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3uhqwjpdk.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3efhkbirg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3dxofqqzj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3qldxkmts.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3pgnivxzu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3jplfkulv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3islzrlmw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zwhuqiwf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3dyjhojkh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3kohmardf.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3lxhizazh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ljtitvch.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3sahoozfc.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3afyawspk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3gyvrzjki.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3iwsonsjd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3jqeyfwby.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3yhqoebnb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3zsotzebs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gydpzruj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3zclguprd.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3lzhmltvh.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3gmhdajkc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3qapkmnxc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3oznlvpim.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3bhguyezz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3iaqzqinf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3tzozajda.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3kggogycu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3mpgtvvyw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vyaaruuh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3rwyalyhe.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ayosiyro.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3smhhjeku.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nqmneasl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3uhadaxob.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3saxapoch.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3jwziixjm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3tsdivksz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3vzbuuuwv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3revodnof.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3flmjsjtr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3shjnkqqe.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3hzzcluae.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3kdbafpnc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3kyydpvkx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3endppmlm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3mtchgjmw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3dnqtkhls.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3rqlxhnbx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ghyhzaku.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3kaakufsj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3woorupkr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3vhhswqjy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3quxqagcg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3aacvxdfo.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hxzkwtkb.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3xqbmcvsk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3eqelzxjd.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3uffciekq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3gindbplg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3klbayfzn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3whykfvtg.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3yjdmtgcu.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3xkbdpxjy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3cpuiytky.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3uatfsati.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3rfnsqeiq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3vrjviybf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3rmsjdkfu.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3druvnqcm.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3uehuplnh.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3slysgorx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ttqeijsc.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3sqslrapb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3lviybalc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3hwgjlsdi.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3xszeobmf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3pdopftrk.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3dcjglspu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zdfhyfgp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jqspitox.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3kkncehol.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dbtwkhoq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hwhynjzm.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3rqubfpzs.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ptzjbkzb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3aoqzavwk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3kddwjlcj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ychjayoc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3kfnbpkil.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cvdzgawq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3hmrjrzxw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ycjgpemz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3sqdxlbug.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3czoqgaba.html


<!-- 参考信息 -->