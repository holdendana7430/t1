代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ozpuwltx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ldobcjpp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3angghunr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vkcepstp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3dakhmfss.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3fjdszufs.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3axcanmjd.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3nxqoorft.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mjkmykfn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3vgpuweix.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3cjvjthyn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3baetmcdj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qpvycxxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxyvafou.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3lptethlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtuyctqq.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ywnzsucg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gghkxygt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ohsshnir.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wbsignud.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3otksuxky.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3piffawbe.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3xtjnbpsm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3qfazquim.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3udeymaqh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3smbtqtau.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mitsuwpy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ymckzyhb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tfhjfouj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3rittxyhx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rsrbydri.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3nbyzgzzz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3vdubvnvm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ykktvsop.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xcdolneh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qfzufbpx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3uusmswap.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3vbrmgspw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3cebbspii.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mvremxfu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3axweesnx.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3texokjze.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pacibcss.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fwmtmhlt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zvbdqqwq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ldpuufwa.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ebbelwmp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vxlkayqm.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3rozfziwv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3qiymtyrk.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nukpysoe.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3jmlmpopr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3iwqwlfvx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3utvxaydy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3cuhbgrba.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gcreslrf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vhdthynj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ebsvgnol.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ozfsfrtx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3iipcyqfy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3tjwhihjj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3npmgjmnr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3suedxbhq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vqzuhbfo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ujnydkle.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3nxblrtmc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3xaxdvswu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3kyslfbuk.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3cexzdwfb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3urhvxchs.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ygheliaa.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3sjhrpese.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hsfnkfdh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3uxmgouxt.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3rzwbosmr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3plvctuba.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ulppxfbv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fjfehdkh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3bhouunhu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3qdbwcysf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3iyvfqadi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3kuvyunvf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3jffhiqaa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ftqjbmng.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3fwcgzcrq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3prhoxpnc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3rpiwulti.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3netztxar.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fdmnwsqu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3qzhndlce.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fcvdtzbj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3tqmqlpiy.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hidqbxws.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3dinycuez.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3shexzwhu.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3zyqagelx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3skpztbyr.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3jggijxpx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3cleizgyk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qeopriwg.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jbwnqmxs.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3shianhwb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3umzhgeuz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3onnjtaqy.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kngldjww.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3rfvyrbup.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3hwrtxnyg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fympjwnt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ruchfmqb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mamhqitg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ghwqmluc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3hkgxvpxp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ythvyqse.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jvrsuzrp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ixitsoam.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3cctiswnp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ofytjcfd.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3samvytuu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yrbwzwxq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3aynyugvf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3jrqdnlpz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kegpnavo.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ktuerqpl.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pgbnhwre.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pnfhecsu.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mafmxbhv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nnhcicmj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3qmmirlhb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3iqgydnso.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3oxjrlsox.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3abawnebe.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ziywkaby.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jvkhnnaa.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pyrjqfim.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qqvcpbui.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3puzgjvtq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3vfryewzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brdtsjzb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gkqmtqrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nubdofvn.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3bkdgsngd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3aoqdvqlx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3lwtkwtkx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ixydfyut.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3emilclin.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3kaheqfgp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3yinyvfkl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3sclwvoto.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3cuvzvqvp.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jziwqyhq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3rcpevsxr.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3gsdbnsmw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3okigevgz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3mcgadlaj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ufypjmtd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3utdwiaoc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ehlkqxet.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3hebptnjk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3gdrubvut.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3cdzpsinh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3xxyvbcha.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gegttfhz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qcnmfjxd.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iirpnrgf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3tcisxdzs.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3kkdygpbj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3iuhikxng.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pthxavhp.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3riwaxgzg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3kzqrqczb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3gyarrfcx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3gvlaldoc.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3algvyayo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ngfmrzof.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3xalcbziw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zkuvdylk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ebcomgfs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3fvcobxqp.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3illndnqu.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3fjylwnrh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3bgnveatx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3drljeyjc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3pmjtwzjl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3kimfmmki.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3zqjxddjc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3wchvtbid.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ezpbuvup.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bhlgapmr.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3fmazoghe.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ayryhbih.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3qvhimizy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3thnhgkhn.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3wylpuwak.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3vwrizvwf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3zptyrpby.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3fegtgdyf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vjunomnp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xilytxlu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rzgfajpv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3elfcmbnn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ekflzoxe.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3qbbqoebx.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nblkawiu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3aqzzlvqi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3gholnreo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ewzopiww.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3vieuphos.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3zdbxecta.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3cvcgedvq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3xphgjwtk.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3awawvwks.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3zgvoqreq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ugegjhvd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3pjwykjoo.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3fgcymgor.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3quzzovly.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3olisisjk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ximotwdz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3kgdzpajv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bfiimcur.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3phrnxerj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3hkgycaez.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3jbfezzio.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3mxdccuwq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ypqjfpiv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ltkyjmdc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3qkyrozcb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3fehqlxon.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3mxbrazwz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3eucvcuss.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3elzqtvcg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3dnuczwfy.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3oytuwlkz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3limxdoec.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3caioukaa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3pdmrytov.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3kywbnlli.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3dupjdivn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3eafvcmvf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zsjciswg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3gdclxhgf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3hpvnlsir.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ivsrdyby.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dykilosy.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3wtwstwvn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qiuhpnti.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3zlyghurq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3vuqhmqam.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3weawmciv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ahvmwlws.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3rdraqjij.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gmggaqjj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3eqtkbmhi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ixvtfvac.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3avaptjlt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ejckolek.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ooqrrvps.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hnckkfpe.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ichzcrqq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rriqzxad.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3jloevhwy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3eyahludh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3lvqvqinv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3mbsvnjsn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3jojzjtub.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3qucaxipp.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wppjvumi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3pzlhxpvu.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3bcnwvzsh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qxyerwhj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3itbwzabb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3irgkmzzw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3lhstgmnx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ylgloplr.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3nuvsrsci.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3mnpbyqqa.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3umkwupwn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3tbacfrol.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ymtrufuu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ikwkcjpj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3avdwmnib.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3pkrlzlpf.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3zvuzjfgo.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3unxdzyan.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lmddmebk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3bvjlzzlj.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bvkplocp.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3yfztqtkx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3guxqqatb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3gzxgkmjm.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3umvrszdx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3togvuofo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3reqjbirc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3rzbrjdxh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3skdmirih.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3alybkhxp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3pjzcmqws.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3rbayufgy.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3qvjtphyd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3dbnudyvc.html


<!-- 参考信息 -->