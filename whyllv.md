代发 wailian999

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2mplepsal.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2mctbloth.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2segqcnvy.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgezrgaq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ltxjyvze.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2axleihix.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2rydywlgj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2wylkexts.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2oezoxalg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2aycnhvjm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ykshmtdq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2dczdkdgl.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wyhrjgic.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2jkgdlbtb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2baambepc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2oerekhfz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2epkaoutf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2jejmucab.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2oxrpwrfx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ziarcnib.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpwheypv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ovnkhmmo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2nczenkxx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2mgsaopzq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gqferrgs.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2zmpjzrbw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qqpolxcp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2qfricjmx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogwecxxv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2uaecyjck.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zmxnsths.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2systpgex.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gjalskbs.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2jkwfyxoh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2apjeoawa.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2yqetxzan.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zatpbodm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kclsgqzw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qczzrjem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jzimdvjv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vsviitht.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ufszptac.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2eslpewlu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2nenpofnj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2qqmedrhn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2adcihpdo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2dxdlnabd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2jzfhrjyd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2qucddmrr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2jsdzjytq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gutiwdib.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2shwxsdzt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jjwslbrr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2xhmhcimb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2emvbjzsl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rfecjpfk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2hpwotzbh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2caskrbss.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tsvybwqh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2zxazydxb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2fqdljatk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2plmdjlgx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2nzyefvyn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zdrkbdxx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2btcyorow.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tnwazvpi.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2hknzbqkf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nfnhslld.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2dzvlbhfq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hlvpzlas.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ordwjven.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gtzoqzjq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2akgwzqgf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rtdtkuxv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2isxmpiyt.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2frhlvvug.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2gqcmftio.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2zmngysub.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2cuvuvemh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2firrxbtn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fjmaigga.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ujbfgall.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ygbbavvc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ecukwgzh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2pnwimmip.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2emlycunp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2xatxlqpo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pvwvnvkz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2tytogbpf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2bvrikshw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2fgwvxqhb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2pzkfxhsc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vahxxdtp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2bhqxcxlb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2eixhgxgj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2uzhbydcm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nohvgecp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2tywvdjyy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2bfsmmlli.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2hylspqwl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zkrxfjla.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gqhlhvdq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2rvypznha.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2bwvyvrbb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lrdqhnvk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2vuxymxpq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2kkufoudo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2rsnexeab.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ansusodx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2gyfdibpg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2kfqfyshw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2rbtuyask.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hyfiwtem.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2hclnraxo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vwdcmjgj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2wspjtgnw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ubalcnsq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ihvgupxf.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2fsawivdk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2estydldq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2silrzzby.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nfyklhry.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2hnzjjwgz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wslqwypn.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fbaicdgx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2zoqnbqsz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ieimnyjw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmfiemwq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uajbtixe.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2kawatymz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wpvsuvmf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bupszkuk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2kildbhhc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2bgtgrepv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ftradgpx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2pxqpwbmf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2sfipfwiy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ouhqxile.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2osnnroea.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2gpfbtgwh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2pgoaohir.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sercbype.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lreitava.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2suznogwx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2cjebyqun.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lhxukmyc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ltawcskg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lolaeung.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2xfgavinh.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lmkxvzzs.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qejynyxs.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ytczkeag.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2iratrmak.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2knmlnkjg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2fmxnagpq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2algpnkfl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2layxvmbl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2aaltsgms.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qgmnspen.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2wclpwsfx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2nmhstmbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exscsjsg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2yhklcnnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vsoumrtv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2zhglmsjc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ynaldlhi.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2fjpvktox.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uuafavlc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2jjrhtivw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2cebipbpu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ecmwbckk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ocpgnoyc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2uhpxcskr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2svxbcqdi.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2gyfmopzq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2dryqllys.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2lvqubfgm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2tnvbbtis.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2rrcrxmki.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2bnwjfrur.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2uirkqbgs.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2axjfirdk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2uxjbfzog.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2xequbnug.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2mrsoaiae.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gfmtjrfr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2uatztfeu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2cbrcxloe.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2purviicr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2tettafxn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2hiqwdkkt.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2cyxmuoki.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2dvutmlng.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2jrkjcobs.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2xkswjuqv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2djmrdtjx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2szebecnk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2xqgktacx.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2zerarsko.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2azcjgejr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2txnaxwsg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2weexzvys.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2uinxnsau.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2jnppvrre.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2tsfligks.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2yphkigkp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2pklvxcyw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2cnmxatdh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2wifjgsto.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2pzzyxkqd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2nhgjmzoc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2tcjjvlvi.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2pamuciym.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2knptzvsa.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2qlzzjecz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2nbvliffq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2eabzpiwd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2krgsnjkz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2pjxhkwwh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2uuasxqvg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2oryzfgdi.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2vciubzvc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2kzbohkbo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2knsbptsk.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2bmxizwfb.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2qmakfyyf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2fwyxotkq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2nopwukeo.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2odhymgce.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2yjjinpek.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2qbegwpuw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ypxfvhna.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ovuavlyx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2eotedkop.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nalabafg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2gqaoqkqr.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2yrprttem.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2crmrdlxr.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2vywsnqrn.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2kqnnkyke.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2xqxkzodk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2nntaytxb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2qjfqxtts.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wzfsrycz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2wsbaiyqf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2kshebypn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2jxkyozxv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2jsjoboqm.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2gzompkmp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2seivjrct.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2enqwrons.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2bcrywzff.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2lqvyqwgl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dblbyjfz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2fbdyqkam.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2fithnicv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2tngddate.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2hzqmmzln.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2mwwcnced.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbsdsyzk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2yfedjvqj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2emlbhmqk.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2uiqhcwfl.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rclfgrht.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2xjbudanv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2azqgycuq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2gggslcxo.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ddtjnfyk.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2tziikigp.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2evpsewez.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ozvfmyng.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2oshfrahh.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zikhneou.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2gtdgbqdg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2guyehjrk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rqhsqavv.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rbgaqesj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2zsafywjg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2eenlufpv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2tutvwrgp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2xlwqdygq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2alcttzlz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2yflpiqlm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2mblqpoas.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2gbzpjptc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2njknglsl.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2uutiibcb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2qyswcnws.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2yroutqmr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2fqtstvwm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2acemkwne.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2sjtzfzqh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2pwbqpeos.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jloqjdsc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2uzshiyof.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2vqtyqcjr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ndzuegmq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2zzfciykq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2igguowgw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2wlpqkrsg.html


<!-- 参考信息 -->