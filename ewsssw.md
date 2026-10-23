代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3imqntlus.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ngomxrps.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3diofdlxg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3pawcnxif.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lclcufjc.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3sukcxinb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oxmxjezm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3wsyrscls.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3vzmylstc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3fatnepyi.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bdmbnzdj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3iilnypmy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qfgskqsz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3wvpfyjdx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3qynagdzd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3wugnjnsy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3uhsyzaig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jyrqliva.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3bzkgtovd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pryfmxpk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eqwctfja.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3anwikmqx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3owfnhawr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3qfzgmxdq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3hymvlfcr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ympnyomd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3lvhqdtco.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3inejyimd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3dngwbjug.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3hiettwld.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qrlnmuoy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cswfzwye.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cymqilfm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3eqnkuisa.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3dikeptur.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dqmggllp.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3sncdwosq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3bxzwkbch.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pyhjrplc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3nuygdovj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3qdgnbuuf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ldezszek.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3kqqitvsb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qjroseza.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ntqkmwat.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3kanabkxp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ltugdchf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3dpdbxpuj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3kqfdqrij.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vywbyonn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pwlntogx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rqclblan.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3gxauzmeb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ctqeynrf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ufiskmdr.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3dncndhaq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3xrazwfcx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3wjrrcjcw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3xwdeloje.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3vaewyygz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3aomqgsqu.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3lugzixhi.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3jrkbtcvd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qdrkeyzj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3upykvvjo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jljfxwfu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3zfdiiyki.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jnrgmtek.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3prdjudmi.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3oxhnhjzk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3dahsbars.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ehuyzsax.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ydgdsifi.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3dfedcqnl.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ekbcgsni.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3tnykivmh.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xdsjfhrv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3dcgxqhth.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3lxxhftyw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dolbsjmo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dzrgbozj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nfpcbofg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cwvqbrpx.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ojfoxdmb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qgkcemhi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fxadtqjt.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3mpmtkhgi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3lsiemrxq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3zawyissv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hsfmnjit.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3anpekmvx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3syhedqsu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3neysyear.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ovylfwaq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3oocqcuii.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3hnvknujv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eubkdgth.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3izphsafm.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3lhqscpuq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3djwalpoj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jtrzxhpc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3klhzntup.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3lhuqkqiw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3lfjxwngw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mexeushj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3tnjjasdo.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3embfzxgg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3jhisyzgs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uzxrnhwy.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3bbyinria.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3dogywztv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3blibwbpf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3minpospg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3fsjuaqhz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zuujfxya.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3kqtnejko.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3amegxttn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wpcuxhhz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lnyjajfr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3efxisfdp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyagllea.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qwadjiwk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hibozysa.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lamhsogc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3urqnmmfm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yetybzro.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wuufxtgt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xigatynw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bwafictq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eiqdcfmd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3glaeppmc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3exzwoveu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3oepmpkae.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zpxqmdcw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rgxpyikc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3sthendpj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hjrwmbjh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3qqhtxnwl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3skdbcvvq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3thfnmejv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ffevdnuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmgncami.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zynittbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3agsffvlz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ofgurdpg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3udkyedqn.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ljjjrrru.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3fposolbb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ykorfebb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3taqpnvdl.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ekwnthke.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3hvdxsqul.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3pqqxbmql.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gmnoqprl.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3qyjwbket.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3vipvflgo.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3pgsgohqb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3riqsrohz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ycfldedy.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3lwlesvtu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3dxameodh.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3iozayley.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3exhtkkra.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3stzyyvym.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jhfrbqpq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3anwpjvkk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3sbwgnwsw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3arekigpp.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hbqymdey.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3yfybqeze.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ebcdmzmh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qyrmmifp.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3wewcxykh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3tcbhajjm.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3mzeivnwx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3vegxkndn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3qephhbzf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qnumperh.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3nlzrwget.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ouvrtcvv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3yxxdpylt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3fvxeqvzo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3mhcxcpjf.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3umxzdous.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3xjqcfamf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3yxqdjtfa.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3suhvnyoc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3qdfwfhca.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3szbzgbbz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ogmuokps.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3gviptdcl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3soqbiioc.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3cwtnqkzd.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3urycbpca.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3tdaixxsw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3hjwxypjz.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3nlslgymv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3oalnhwsn.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3zepiaydl.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3qeaohmhs.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vcuewcqi.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3odsjwixt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3vmslujwn.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cgtverbh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3srykvsbo.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3wwvaaydq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3mrphmauo.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3dnksldgg.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3jqvnecul.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3wdypxozg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3mrppndos.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ahvmssgj.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ojjonddc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3iwthjaub.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kszjfxiq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3qbezlfmb.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3xuuysiex.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3mhtrilqu.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3wwwgshfk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3igmorarh.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3moamjccw.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3bqzvtssu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3rbgxtkyw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lzcyudcc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3jqnulmii.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3pscgsase.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3hlhcmxdr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3nfzjjfmr.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lvrxyxso.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3scqypzyl.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3zttiabfn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ckyoigys.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3znzynalo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3unqtadsc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3molcbpkq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3fiqjofzw.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3crppcdlx.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3bbvmcrhw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xolaaqhw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsggieui.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3gaglfwtc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3zvkbpiov.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3hkjhysjt.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrahwpyi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3pnhajcxd.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3bjlzdqnk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3spwctwks.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3nxpfnven.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3dzjyjnmb.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3zfnbscrp.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3qlxsbsqf.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3rosurlcn.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3crembizj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3lifihuyw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3jrgwbljf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rfdmvgsm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kkmkinhq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3qxqayozt.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3lvlbippx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3oxxwzaxd.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3lshtygaz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3trtrtqte.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3qmwymzns.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cqwaqbvf.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3svvovcje.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ygdckdre.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3uwoyalhd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3nizrkkub.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3shmrwhnu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3omibdkwt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gnpvhxsv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3lxifsjbr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3tmrpfllj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vtadmwnm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3wodoufpq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jaeydpyd.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3qkfyhznh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3liavxelr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3cxfapqdh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kaqeribx.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3yhzsiwye.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3pgjzfjfv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3vwuggvlh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ulfdcxgf.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hkgavysv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zplinodk.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3mbrfyxkk.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3czsbwhon.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3yfkdnsij.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ueywxeml.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3vhwvcdeg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3agbtmstc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3tatpnpov.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3oldakcxq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3utdsjlnu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3pmyemulh.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3dtxfkhsa.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3drsnvhjj.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3greqizgs.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3wszqzjze.html


<!-- 参考信息 -->