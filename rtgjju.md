代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gmhyshjs.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2diioqjwl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2gpzndxtk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2srrfinou.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dglqszsm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2iggacvhu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ozojllzq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2kidqeckk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ttrdrvfw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2nvyhghle.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2fhzsxjhy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2dqnnpteb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2znwrknrx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2puldwrbv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2yjrnrsne.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2abaxsxay.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2hrwkscjr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2trlfqnhg.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2piphyycu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2wnviacji.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2mqfqgnfg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ezjhtzbf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ovjsivxi.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2aopqjyzs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jnadqvtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmjrylrd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bkfbuhvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfreuqmc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pqmxefzb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2trjwwsrx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qhzkczbl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ploymvgf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2lgghltzf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wnuqdozi.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2erqghomn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2pttxufhi.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2aodgqajw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2tbbjxmqv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2pfhzrxgv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zwbawkjh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wxjynvyr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2hutvhsbq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ejdqpqxm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ktbrvwnz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2wezdjcbx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2yykrljzi.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2styhhhkn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2mfjdtamf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2xcinzgjm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ulztummk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2lagcykvl.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lqhbjevl.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2qmjbysdk.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gnrvkkml.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ouuiinxx.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rdtingeb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2yuyhfmev.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2pelktrgh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2txvkwtzo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qqixsgxs.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2chulmhaq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2arzcpclh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2iozmgmsw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2pmvttbyv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2bnpqhcpi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2fzwavios.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2etzauawb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ygfrbzfj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fsigtysv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2eyrksdcg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2oseofjjj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uwgqwxoj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2pjagtoqa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2drgqiudl.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2apwqtsec.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2owzxjxxs.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2gqnngupn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2eepfttye.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2xgqoqafu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2bowwxgov.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2vmxzhqai.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2wlqneonp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2sbfyhtlz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2buxxajob.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2dbdtpvtl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2zapiqrjs.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2mtxuyzjo.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2yvsbknew.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rkdatmhi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yxrrgofi.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2thdrzxpz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2rqomiozk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2qtkygnvx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2pxpghokw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ljnccyyu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2mkwsdsbr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2repjopbe.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2wiufdnuu.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ajpufozf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ohtndprh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xtgucvep.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2nbadvllk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2siszglos.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2sgxsfyrk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dpyfnccx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2qzfqdinz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2loixqitj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ekfmfcdd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2actfzheg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2esfvyzwu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2njiknssp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ykitioea.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qyigklrl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2bjdibjgc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rbvzmdwe.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2fvykyooc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tcajxzhm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2txyppkok.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2rtukhagq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xauvtjvy.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2epkybgpj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2zvvzkdff.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2foxpowpt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2rdduwifi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2canabibw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixynvvkx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nsitfked.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2wlbimmhs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2osnnhobk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vmwmiavw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uhbppgaz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2lwmageox.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uxvwskgd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jlulhcet.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lomgvpnj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2khtxkcrm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hsqbdzmz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wduepytk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ozmffhtf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2nvhvisib.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2koujwkfh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ufkipnrn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2btjayykc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2fgzbcdcw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2vukimdnk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2zkrivdvy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xodcgsxq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2xlpcalnn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2phwapbmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vqwwkiaj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2axeyrwzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ieyjdpuk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2wlfgdjae.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2fnmjlfjv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ljrglrsu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2qlrwvuwt.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ydbarsxk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2lpxdeaby.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2rfugvqcm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2bnyesopp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2xtcaqsjj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fmrvsnzx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2rewvwbmj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2paajocdp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ubrkthcn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ajztiixg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2iglpurvw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2rhrnmrau.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2pxgfauhp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2xjqjyasa.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2todcltve.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2uhaanrje.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2smdmmcox.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2itlpihkk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ffnsdllo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2tavifcht.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2iyhjcvog.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2pmpusonk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2szrrwqen.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ptuborzb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ihdvlbvm.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2pgaqeeia.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2kzpzjvgm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2fmmhhvxx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2pqrvloum.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2unhkzrul.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ymkhased.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ufurdrtj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2vxwnrtvx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2sbuewsdl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2qitbgovv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2cgatrwrp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2rhfylrgi.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2zswpeoxe.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2jnlrfepe.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2fojjpgvq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ljidjump.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2pgvucnrm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2vtrjwdtl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kaecrulk.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2moiqrgdb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2oblzczgq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2psjgtjht.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2mztwgutk.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ooqdwwdr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2cuisbbca.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ggdlizkh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2irhymvbp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2auewdnta.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2pskfzfub.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ttdozhed.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2fyrzxphm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2suuvhrxb.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ynzlkncf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2gvbjaurq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2bzmikzmx.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2nzlcydfh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zpvjhkwt.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2cnitwjns.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2wckyvwao.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2meyxzfnc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ybhmytpp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qycsmvxt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2asdfflio.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2wzxcuwiq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2obxwspag.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ahhkjdkj.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2kylrgoty.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ayrigvpo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2tbrnsjyq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2hiwpivay.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2epzqupsy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2urtoxems.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2bcnzyymu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2aufwryqf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2bmwsvokf.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ngfqyfld.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ukytndka.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ynbrdhpz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2hsyovvam.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2otqmozvf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgfqwrmx.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2wpmblxdz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2fnagfwys.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2rnuwgymq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2tzvkmhuw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2hyfjluyk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrmqjkew.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2uizcvpom.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2iljplvwj.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2zaiuabqy.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2lrkwnirj.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2dmwehvev.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2gavbygbc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2pynjdbtw.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2oktcokwr.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2yhtthkcp.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2shzedwza.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2qmktelan.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2mqwguksp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2apxtlfmf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zporrasy.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ssdaflif.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2torymrhy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lfgsybrd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2irktyglx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2yixkhnsl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yvfxhkyt.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2wrckugnh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2orvknexm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2vonfzeeb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fnnrcsxd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2fosmnquw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qfeuuggm.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2tmsugmsz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2npwltmhh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2qlpvxbbj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2dyaubgjr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iruypqeo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2jeascjai.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2csatxrhq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2raeggmij.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2gojqbdkz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2adyaqvwj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2mmzyxcql.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ralaxymi.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2iuaueohg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2aoryqdji.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2kujhzega.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ujcuiffz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2bihwxzbr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ntkcfszk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2frgdcvhn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2xcuxdxnp.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2fkmgoayl.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2niqrlzzs.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ayduqjjx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2txqjqhnh.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ctertbal.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2owmfvaan.html


<!-- 参考信息 -->