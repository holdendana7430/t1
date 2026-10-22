代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rdqkpygq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2frojgjeq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2flblvgkp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2jinfihce.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ceziybby.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2kzhjaqqj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2mxvgdshw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2vhhzocbj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ikyhmsrl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2xxopozht.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2dnlbiynm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2nfudnodz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2jutaxacp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2snsdedzs.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ycyttebe.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hwuyzxes.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2lkmzttmw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2pftihdpn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2oqrsqfne.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2dxzsjxru.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kampklzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qsekxefc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2tallsazn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhedhmxi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2edmmfnre.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kjwpkssd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ayypfhgi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2cwyeqgyc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qpdqlxfv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hlwqifbi.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2azklmuiv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2khfmlela.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ilfwxzjd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2xnexnzcr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2orssgxgk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2phscibak.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2okmwxyxw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2tavenljf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2tumrtphu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2kzdfzbzj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2fsmvwpzp.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2uqubnqin.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fsuhfaru.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2znsqxxxm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2wsjxkayt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2yaiujfca.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ltmurrxq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvztxxlq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wpvoscpf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2euhjfhyn.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qawbtvcd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ssraxtfb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2qikcktun.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2mcfgdnos.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zstacabz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lysyiype.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2hdciqrlz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2pyopjpwt.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ghgkssiw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2nzkqtzdo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rybjtbna.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2vfzltmec.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2bvxosayi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2nejeicxn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fzribhkl.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2gdokfnvs.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2kavgbnqt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xpwpedhr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qogbxgkg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vifcofgx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2etfdzvms.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dllscysv.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2cqgxmzjm.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vedjlfua.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2mmljcgla.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2xwbwsvcg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2oxmjcdjz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ttarevla.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2mjrnycdk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2uzaglfkf.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ifgbwomt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2odnvfapq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2uqreuhyb.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2flcqrrip.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nojcxamn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dqkvrtuq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2hrejzdwn.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2umscqwhq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zhlsuspc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2kvseqgle.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2stowylpr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2bltntwdi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2iavkenhz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ddhlgsgx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bmaurtgu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2itbswwev.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2phrdzicw.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2nqlartmd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qcwbgjvl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2vxwchnej.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ihouvswo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2rxmukgnt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2bvyigbmq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2kehkwelj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cvqkmqrn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zuuixpue.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2alfjdfpe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tsrvauup.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gqyslxdv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ovhktddf.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2bihbcdjo.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2miwgmrkh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ciisqiyk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuihuhzi.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ghdkzqos.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zddlpyus.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2akdassnh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2yvijcjhj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2yiyzfpjg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ybzhjpob.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2lzquoezx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hjnnmtaw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mmuwvijn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2jhvmovpi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycxsymzh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tcbsmbdn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bfapktpx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2vjufvaqy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tecsvlpn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dafkphcs.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ybjikdyz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pwfahugm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eydslkcw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hepzssmk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymsburfw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2vgrpoirs.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nepxtkeo.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qvoxwwvt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ipgqgzbj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ktfztvng.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lywqfqin.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ypverady.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xixhzork.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2dqvvgsfo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2jicosiwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzchuovt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gtpmqnka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okzfxyye.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2jhchidov.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2nmjmelyk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2docrtlek.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2puiluyuv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2uavgbgsw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2fnjnlvzx.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2rngvrems.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2wawipwuk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2umtuklen.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2butgfsei.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2pfpqxdxb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2diskootx.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2omlllbrq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ytaosuqk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ygsqqaat.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2bfbdtjya.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2hvguptci.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ijycdbnn.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2urdnyngg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2osszjycc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2jblpiuys.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2egzmnahw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2spocghxu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ngijjihv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2fcwwrhoq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2dyjeifpz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2cjaxrrbq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2dxgswtzb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2lohosmjn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2mniokrkp.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2gbvwfeva.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2vxxtacar.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2lljszgey.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2fbllpsoe.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2nfgtmdcy.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2brbeodhq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2vnqayhil.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ssezedls.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2fnwrriea.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2tqnoasdp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2jxfdrxox.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2hbqfmsuk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2raulvdmj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ecvohwwj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2kukgxpnm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2pgbjcqti.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2msrwaqvm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qrnlmdvt.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2xxrdtfjf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2opcwezkh.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ynoqusff.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ghknmksa.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2jsmpeasw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2uutgrifx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2jnuwetpm.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2qfgrckzp.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2sekkxwrl.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2wprvgzgu.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2pvexodqk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xhlukhqu.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2mjwyltdq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2bdiorlww.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2fzioails.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ikfyuzba.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2tvfvyflu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2desnvlhh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2yyomfsrk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2dvoxjfux.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2vfbiaoxs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2wrlobfna.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2hfuvfmed.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2fgzgubja.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2jqohhtqh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2rgqnzpvy.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2sqwgpklk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2yigjqwlk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2lvulazzy.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2vhacvkmw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2gdjnuxjo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2sjlihqrs.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2iwoirlyw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2zwjcyxrk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ybiwzitr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2citonjlk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2gczbozuc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2cujxnpve.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2smdlzysb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2znxipfuz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2lcrmhfye.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ytwvqnsh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2wlyyhwkq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2mxnjpodb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2vpimaisd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2toitwhqf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vbhmqnqo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwixmibp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2iboiaoqe.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ggyeyhjz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2qbamdtrs.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hypbgfzl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2koazcedg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2fhpbfzot.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qlibmmqx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2cgikjeti.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2hutlefoe.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ntbfirnv.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2vydxauaj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ynimfvql.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ldapgyif.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jhywkvis.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ffsezvbi.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dhnrzapm.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yuohbuqv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ldwkldba.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2onjqujye.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dkrdeend.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2ytciphqu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hclcbdtv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2xjujiszc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2hwnkwvtl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2djdalmqj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2owixlldl.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2cisyswui.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2rcgfycph.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2mtudtegs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2cpazkfhg.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2gxhrzwpz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2fhnxffyb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ixcjfhmf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fguecdis.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2mzqobavp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kiindrvh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2rnamnupd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ilvzwggp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2pyuuengf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2rusmvlus.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2sdcmsode.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2glxififv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2ilypqkun.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2wwowfvmp.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fvrjxiid.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2mwqgijms.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2jkzqlsoo.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2cwvwqkqs.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ifwwahjx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ticuebtm.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jlnviute.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2xfdvzytw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2joxiakyy.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2qrpyuhli.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2uzcymdoo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ediryjzt.html


<!-- 参考信息 -->