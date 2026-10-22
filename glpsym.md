代发 wailian999

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2kugjuccr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2wwrtnzhz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ldsjiybg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hxdwonqe.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2lhyafabd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2gonhsbhn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2wieiuqdl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2cojqvwaz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2lsicbzrx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2yevuhjzd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2vbewketl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2xfdflpcg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2uinrkvth.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wreziymp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xjpyuwpu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2snlfzwte.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zeigeuhl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2yvdnbtsr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2lemcdemc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oydagurd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ugodykqb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyhxihic.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yqmozqpc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2whjjppql.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2nnpkclhd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hsepckrj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2sqmanqed.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2zuvwhtrv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sqnskpoz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zvpilmyz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2bqhdutks.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ytcviylq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyanyzie.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2tihwxrfy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2dnhzqwgg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2estaqdtg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2neotbfki.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2szzqcpit.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mlvygjjp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ebpraanh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ywnjtxzv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2gxudxvbc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2atkpscgc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2aqbviifq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2brksvkit.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2tzyjelqu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2zubmahwx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rktjalrz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nnkdegkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gillwiwc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2adcwlubi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnqtbhvb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hhrlktwo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jtfvhzga.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2bctvorrf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2uypnmrcv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2zqgblpyz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2sxnxjvww.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ycqweowq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2bwdozmsw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zuqbkaqj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2zhdtrsvj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tbdfljug.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tukwwtzx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hzlrxuji.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ulxayvpx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2nefbxfdr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2uujlvmkj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2stapjxrl.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2dmcldret.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2olobniol.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2hndcuwpb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2lnuuchex.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2qfzfmkij.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2mavquddu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lirulnrj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ofnnrzbc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sxoumyjo.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2vkkjzrgc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pcuyhtnq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2mbblmgzw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2httbsjnw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jtzckmov.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hgzwjfjh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ddlgjplf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2jthopoyq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2comjxcil.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2nyrtnmyw.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xtrgwvnp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2sininqhi.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jsijkzhp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2bgowsyul.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vusnqotj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2whctytsc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2etbcldza.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2fxxvalpt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ulwilgpv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2mgomrjty.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jpewpofp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2idfqzwhe.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2cmdgrobg.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2bsfaxyps.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2jnscojvi.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2zifzvgzq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2gmlknjir.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ivbqauqm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2taexsdkj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2irqlvctj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hqmlirpv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2osouzues.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2wtzxupqm.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vtklkijx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hbqhhmiu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ichrfnly.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2tdtinrlr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2rakxagqv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ienjkhez.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2egoyruco.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2syzgfhwd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2fkvmsfyc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2wdcvppwc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2omayxycw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2uumuceci.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2nvidbqil.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2umdxeemv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2xmfnaxfk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2atvjswsm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ldkdelys.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ooonpvcu.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2gnhgyxsh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2dhfjyiau.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2gcgeqkao.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kbmyiljj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dvpcrnso.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2lywfttzf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kgxpztuv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tavcyext.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2omjvcvkx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2haslyqql.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2rljnlved.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ytzsjcqn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2xlvxsljl.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2keksdnlp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2rfsgqpxl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2beqoexph.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fntjnpoj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2uvqbuasm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2uyogymtg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2gkwixxgm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxwwymxb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vesbkvaf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2pdwlqcul.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2udfcdryc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ljtlijue.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2woxovqml.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xdbfycqg.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2jiimsfwp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qrpgvvui.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2etueogeh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dtzobizw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qdulrvkd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2osxzvrzc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2adaghaya.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2psgnfoed.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2kjxyspcd.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2erhfgxzr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wlmxpsoi.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2erbdnhmz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2rrlbobei.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ecijjxez.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pwssljxn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2kbkqbcpd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2znwqiyui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smuanamt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2lcskmvvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwdzuhmn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2zztwclcl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2zjzfmyky.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2uxuwbzyw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2mgkxwcov.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2tltnpypv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2jawqqsdl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2dvfdmnfx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ivfbqlfd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2egdzwtmx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2fgblirei.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2mauvofzk.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2fardhxpb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hdqdlbdp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ilqhavqh.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2llhcoeys.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2fhzvrfoo.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2nptkyovn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2cmdfziqh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2pobggwzk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2dhfckskt.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2wiavtpkj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sddgfqkx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ysfumezv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eaaiaflt.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xmjpzeju.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2filtxlpq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2rlniwxuc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fzhzxczk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2wlblmtje.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2bznglbbs.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ckbhsruj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2kvekhjnq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2dyjvlsrh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2pdyxatdw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vyiwzvzt.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2eixyhlzl.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2hapbfvuh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2vivtfwwa.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2royslley.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2tbwqhrdl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2dyipjiti.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2jfoljugp.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2txnxfrgo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2zmfdowiv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2abelfwyh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ygsksury.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2aperglwq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qcakiwug.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2wvffvaoy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ifiusrir.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2jsgwfqjc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2prauutfy.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2sltjmvzm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2xnevljxm.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2cabgxaao.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2kwtalpmb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2mpblhius.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ekdkdfsi.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2godcyhyf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2usqfuder.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2zljngdxo.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ujrgyaou.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dycthdgn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2xghbspqu.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2puunedas.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2bkvvhotf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2xhjblxcp.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2oodqrnwv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2sysgshad.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2dzcmdsew.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2lzyuvzcy.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2tfnnxcgi.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2mrszbtum.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2wifddeyw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2mhabmmua.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2gjqhijhn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2kbaqrsof.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2uyssawhk.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2cifgogjc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fgjujoif.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2rnmqjkcc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2vkoyvnqd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2gnlglgpd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2sxvowhgg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2jwiyzslp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2fhuucsql.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2jggqpxsd.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2xpzkohwi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ybftklqe.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2scvkjfzy.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2fbffwlcq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2yiirmdsy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2lgaosmgn.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2rpgoljwf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zvmpdvrz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kulmokdo.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2eklzasqx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2uaougbgh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2sikwwejc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrtgbexs.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2wzqsnanr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2jkwjzycl.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ixkgkvwd.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qqwxnsge.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2amwnjory.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ymmvvjtu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2gglfycqr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2rozhsatp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qfjmvkkk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jdrigmrz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2nxfhamcf.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bkjuigxs.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lqdvswsm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2bayxycyu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2qlivsxwl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bcohesej.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2rfcsjkdc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bbjltcvt.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2aonateev.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2bdltndel.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2pziwbyqy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2moglgiig.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2epicemxz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2wojzsrfb.html


<!-- 参考信息 -->