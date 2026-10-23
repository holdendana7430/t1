代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3blecwaex.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvsxdgex.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pfiucbdz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ljjjjlhn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3rovwrclj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ezasrckn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3jjjchdcj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3kuohfbtk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3trfwfvbo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ewwqcfxj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3iofxsake.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3pqtezubu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3xwzwloxj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3matkfxje.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ejsmhvcr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3unufcvwe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3rlyakicd.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3mfepneow.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3gyoueqso.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3cbswvmlj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwtqsbqy.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ntvuglrz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vowxikix.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ancjhbys.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3afehuorb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ymidafkf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ukjkxtvb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qrbnzbda.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qlczxvgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggjxdfua.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bgngltjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwfcpdqf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ddlwrmif.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fyenlenm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xlqxcswb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3purhlohq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3xtbekezj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3evgjojbw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3huutkyuf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3atwclgsj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3vubjhiov.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ghiyliwb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mrrbnpch.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ohdfjgzc.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oxthzoke.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3hoffjflk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3qledddmn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ubxwfovl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3yqjdtwvc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3lybzagpo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ovphfcgk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3erhopnmn.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3cnzhodql.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3wpsutmjw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3nfodptro.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jalogumu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3tyifvads.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tsblznvr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3wydtiqry.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ewaccudj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3qfkhkxpp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ytjdlyoy.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3odsxwmop.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3magjuawk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3vosqxywn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3zvgpexpb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zdespknu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3dutkxxwq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qevzvwwe.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3qfxhwpbf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3lbtbkayr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ghqbqhev.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3phdfmyji.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3wcbduvtn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ywgufwqh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3oppkjdin.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nkdjphpb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3kcvmaume.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zanethlb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oqkvmcon.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3malxyfwk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3berrnnqm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3lcoumsxa.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3raimfcqi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dmlfkzud.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3zxqsrvsx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ajabkddj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3yagmizze.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tcsacsvn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3odglvtdw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3hoobpgsg.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lfymhiey.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nkoeyzlt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xnbeblvw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xcywmsoa.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3lteahogr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3czykspvh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3okgykqgu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qkfvnrzs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3albhdcdf.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3kyzoddpa.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ykprmpog.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3epgljyun.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3hpewptgx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rgtizfop.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3kleprqbq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3evywpkrk.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3uwzrchje.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3azroxtfo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ytexbrek.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3hgujcsyf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3rwfrefbq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zgknlwvo.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3sdpiscdn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ackvgspd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pfbtucle.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kimkwpsf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bzeyfhzz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3hlnxvrvq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwheuhpr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lohdtker.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3vxwtawnh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3qzrntinu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvbwvgsd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3vyvkbahp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3sstjzwvv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vjkdtehc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3akwnvtrb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qurxdajb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ghnmebqf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3csmwgrjz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3nfyusaer.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3fkbqpele.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nzsrtzjz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rjecwtnp.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3yoraiohv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vgsvalhg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ywfxaqaj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ybvjhbmx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3aknsuroh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3lqzbhquu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vpepxble.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3crfastol.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3nwzdssfg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3zenfjldm.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wrovxkfo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kblaquma.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3aklbfrle.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xqmjrqyp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kywtbgey.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pkybehcq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3cydwejnl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3xddphcln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rttvtdrn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3owjsmxca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzvvqezn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3sdrqjzbt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3pmzufvis.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3jijpfymj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3agfofzxt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vmsinsov.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3iqtaaozw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3nvolgdzm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3bwvppozl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3fisjtfak.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3emriukgk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3fltjdphj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3cxvboknb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3rssajujw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ofwittfm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3kufczrab.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3lqnlpptw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3lwepwzgk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3rzpycoqa.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3oznvcatv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3tfxzchvs.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3isgrozkw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3hasghpuz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3imgaxktj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ynivxtac.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ircwpsrh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3jfttoyuq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3rchlackm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3arttozyz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3vmsizxxe.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3yqotwfwn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3wgfzkljk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3mjdjuyvq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3mgsrosih.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3unfezzpe.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3mxuboaaq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gcxfvayp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3sgpnczmu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ccluaand.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3sesbsqky.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ajyfyujx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3twfxhacn.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3lgzrztui.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3fbrfrjdw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3tpuwrtcz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3fetpzzwl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3vpuyksdp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3cwlziotj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pedzdola.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3tvzhoxjd.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3nzrpzamd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3hymkcjjp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ewotqvsl.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3hwbetres.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3pzxbpfzb.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3qkzampjb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3miykdhrh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3wtdllqrh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3bybbdpsd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3snwlalst.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3mpjvkdaa.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3hlrykdnb.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3admhsinn.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3wgvxzddp.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ktdgevpp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3quunjoia.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3dftzzevn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3nbzzwggu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3gcruhuft.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3qrghgrvr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3zbkwpxid.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qaggoxmg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3xiowwhzy.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3dpxopkdh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3byuwhuxe.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ohpmonuf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3iffnyypw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3recpccpq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3yhgfadfc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3nqdglluj.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ofehwohs.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3hpuwufuy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3kolvqupu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3qknxeugn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3fuwfuuld.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3nwkxoebn.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3fctbfkxq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3edmwkimu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3kofijvyr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3zcgbydfh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzrtvbrk.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3mzjmxdmc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3owmrnjjw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3veazkmmn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3exjkrdua.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3felgqrqd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uenxkzfb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3uptpnnwv.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ucstzmkh.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3namojvvj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3epervlwm.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ljhodwuj.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3bzbrhzqe.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ggumzyya.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cyyssare.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3vrjuvvcc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ecknvngn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3htxhrrke.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3njrsbqcc.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3vrckrmgn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3hlfmxbfb.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3keryehhk.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3npvhnzlb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ymookjac.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3cnmvuoba.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3vnfeaelg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3axbsugnv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3gwhjengq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hvkimkie.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3vmsfisll.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qxutjhck.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ldzocqzf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nvbdynqb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3cqsctjtq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3tikycbla.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3qnhtifcx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3tmbdljza.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jvuqhazu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3zjjbnaot.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3sbwszeey.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cagykbwg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3wlflrwqo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3agwfudqs.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3dhxtnecg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3vrxupvjv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3kpjykkvx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3bxndbjys.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3xokfahec.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3hotwkygj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ppvgtwhh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3whmjjygg.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3upmvjgsi.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dyjubugt.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3gtfxqkfv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qlbqtjjo.html


<!-- 参考信息 -->