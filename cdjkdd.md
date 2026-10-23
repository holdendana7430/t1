代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vmegfzzi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxeqlqut.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bqzmyqdb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3bsoyabhc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tpfmolds.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3sxrdrwby.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zxizwsja.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3kusqtmao.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3icktxysy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3aqdeoobj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3rysvjgsz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3dadnybro.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofzephzl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3moyiiopy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3yfjrrpwo.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3cdxtzmuz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3bnxezlav.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3qirqwauo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jyhhoepv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3loxsoruz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkjmjkxh.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ajobdbmg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3aqqyquxs.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qlllpobc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jxwnjbil.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3dkwabsda.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3vfzkgwhe.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xtfuwqos.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3hioyqosw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcdajppm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mefrgwfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3awypkhwj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3euoocmhz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gyugjwcn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3iakufqfn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3fkmaaaqa.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3bivpqjhx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cubbrjgs.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3jdsmyehi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3nxymfgrv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uemsrkeq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3dkoukurp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3iqohkzii.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nzvymdzk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3advxpgjc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3xpjnjtgy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3plsupsgk.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pkyctika.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3xwdmrbpa.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3vxwpssup.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jtrztspy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3skisdfhi.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ctdpoeav.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3egjgwjyk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ozevtajk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yrmwtfvs.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ercxszvz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lwiqxitr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3saupmgiq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bymdmswl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3zzbjvxlw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kelhkhbt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3paykvydw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3osutexzv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3gdbsxtov.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3qsbnxkdo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3srtxfqxn.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3yupqpndj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xvwmofoj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3jrangvra.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3toesqtuj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3okgwcfns.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3igycozml.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3cphsstzo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3lyosyays.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ueptstwe.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rurjeykq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3kenqsdwh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3fgxvkrjc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3butweuuo.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3dfdakzsg.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3mocpistb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3svdtagro.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3vtvxfqmb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mukqggzs.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3dagvwmcw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ddmdjdhh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3urtghrpr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3jcnpuojn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3lbxvvabf.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3nwuedbka.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wdgokawv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tssfvfyn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mnhxwhuy.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xbgkcdcv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cfgfunnx.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hyburoqn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3wqwxvunn.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3uewqpaia.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3dnaioftw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3btycfqng.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3unsdnvye.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qktyffot.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3njaxwdkr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3tnbkmloc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3rgvledou.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bprfnpni.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3kzjqbkjs.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3psticdxk.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bdrtpizp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3qlphihbp.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3edwoafbv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ltffucvj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3wpcrhqyl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ifdtxtss.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rxzzqzvy.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xlqasfum.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3cgzzvjxq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ikjwmivc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3imirjrol.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ahaxbpke.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3xjwzcnfs.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3bzikhcqg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3qllspyxi.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ehioegwt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3rpclxvyw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ushmjiuz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3slssdrbl.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3einieqvx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hjhivlmh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3alkvfuww.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3tnueqtdg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3vxswxbbo.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cujkjncc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kfasrdck.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xfdcmtkn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3krspgoil.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3oflxjtsr.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3brcecuux.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fjkdbcic.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3olbywlbw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3edvsgdua.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3soykfnik.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tqvtdebz.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cdvyqqip.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3eqmdupyy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hpprnjzh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3jcxjgtxj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3poxejcqi.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ezlnwfis.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uklqxdpa.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3aaswacuv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3jgzatwgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3msjjfbnd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nwuvpchd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxmzpwpm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3rdzffndd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3bhainryf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3frleemos.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3drjwzkco.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3jmjiqivy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3kbsfklwk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3dowlqqkl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3gpgiwwud.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3udccosxc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3janowlwk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ixctlfrs.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3cxndveip.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3rstzpppv.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3rskchrna.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3sszfvbao.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3bznhiari.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3nqjjekmb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xieczqrt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3kelasnoi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3qlwyxsku.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rgzngvaf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jkuoqdlb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3awyipwjw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ubfuavco.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3skzwzrxt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3wiykfwsj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3pphrjurk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dmaxbjxz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3xbecszfx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3wqzjvirb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3stdlewnw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3xjwbfcsb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3fvsdzjcf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3qvqqaiac.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3uhmnmvda.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ymnubcvo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3jcmphrci.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3emgphhyv.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3okanjlrg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3tmsljmve.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3rwlafwrd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3btiaotmc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3dsarnhhs.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ziwytgaj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3kpfwpuvz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3kxjdmsco.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3qrlfzcsr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kygkonhh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3abexpure.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3fzweuxgp.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3hlzcovsd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3qyuivvup.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ktebrfao.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3jmcdkklq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3udselgdr.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3qaqggogj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3xvghkdre.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ecadzuit.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3svdffvqi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ykrvmwhy.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3xxcyngpg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3weqlhkqm.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zvxkinsv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ndwxmaek.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3pkeovpld.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3oglefqlp.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ycmyuyru.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3dvdciznk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3yaogprzi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3urpmmwyn.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3jantwowg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3bctjcixk.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3vjfucvkz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ixpruyna.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3zjiaefrw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3lqfayxqt.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3tdgombvp.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3soifrrya.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3yglsjibu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3yafngbpu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3bffziqhf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3mwghyxvy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3bmelxfgv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3mqrfmipt.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ynbuxlrd.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3qabcauki.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3avtkrhzb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3sjqtxhca.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3hqvgrwzx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibeyvgqg.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3lgqtxpad.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3fqqgqivz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3qmbdefri.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3wzqbekvl.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dnvdvvdz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gviskznj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3cmopuzzs.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3kdylfyjl.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3gvojrarq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3qbbotwbd.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3kdkjwhma.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3cgtpmjza.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rpjfxgse.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jjmezknl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3iqjlkfid.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3cgybneem.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3dfhzmlyq.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3eydnpldo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3gbsmpopo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ddiimhxv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3pjaqgapb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ekimudll.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mtzkiart.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xjquorcr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3jhkqhuum.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3zouxqjni.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3xhnezezu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qkfkqfix.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3vhkcfvkt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3wluwfajv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3imihfsmc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jbwrncst.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3npwjlyrc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3vrecqvpu.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3niwbjrxh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3oppjgpvv.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fcnrxblp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3mcbulutw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3yqwstnyh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nbasoikc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3vybszgaj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3lcdebpgz.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3cvyvkdon.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3wodcjxik.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3zylvadqc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3xzjrqyrt.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3epfpgwkl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3yrxentdv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3lzavrvac.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3qlmlvong.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3behfjlee.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3epsyzmjf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3luogsppd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3rxcyqumd.html


<!-- 参考信息 -->