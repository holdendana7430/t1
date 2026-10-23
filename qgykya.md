代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bbugcgma.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3vkotgpww.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3yczfdkjm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qagjvgrl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hsslrkfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzczppvj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ercfhtxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kafrbfkl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fvmfwrha.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zvicccwj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3wenqvljo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3xitlyeuo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3eglwyyuw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3sqtxqyjf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3shakfsvp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3gdtapbee.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wfyaqfck.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3jzzazupn.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hwlnvqik.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eadpvhot.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rwhoeisb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3uvpwcvmd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3anaeokvy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3muftcjib.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3llircsys.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3lwsifwvy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ivmrfubp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3eneypgfq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3afqffkoh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3lxjcdwgv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3tcvrdnpe.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3imtnbtqk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3kzdoexwo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ppfofota.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kptrxlkv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3fqbopuhm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3bjnvlvqc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3tlpwunxa.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xzbghtuz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dvfrbeiu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3aqplhrqm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3rieycicn.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cdswlavu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ioavxsqp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pyfrhioz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ykmmlusf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3jdviamfv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3uqbrpzda.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3acupvwve.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zvhwhfqj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3lnuzbydh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uxrzxzbo.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qkahnbdl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mvzljxrz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bwagixje.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rlttxoqj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3grqytowg.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ejxqphmj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3gbqmragv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qziovwhx.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3mtveeizg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3mtbnwrju.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rcdprzlu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3csdyuhky.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3zuqwgstp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3gwpfkppe.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3eynrabaz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3igfdxoor.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qjgvrtzi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vmpqrlxq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mgmxhjoj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3yzeayzzz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qeeisjwk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3efwsydqd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hfljwevn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3supiikga.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3zduarwva.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3glbmjiqg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3znwipkbj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3lxogedia.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vvifuypr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3uvmtcrgk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3yynaidlt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3eeophgxo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nseluuxw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3pedmztuy.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ixfmhwla.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3bkgydbms.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nrrjtmuo.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cndnvqot.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ndqgkzbf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ylenwcpx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rmgelenx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3dadyfxgm.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3lvjuusst.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqpqgdud.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nzspbgxo.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3bhcbhdrp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ircjifvy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3embaxdhs.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3dnyraniz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3rqrtbapt.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ovyrivkv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3zegtuswx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wizkldez.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3okaunzrp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xbvwzaxf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3kazngiyl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3epamzbnz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oavafjta.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3upalrpjt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3gxklxaek.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3oempmdnf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uhgzahhg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yylvpzyt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mcukbmpv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajeswtbf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xpvgedgr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3wrsnjkzp.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3fzwguswl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3oivcolgo.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hqappwvr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3mysmkdqn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3owqmbvqm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lbaodjln.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zvezuttq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uyzyuuxy.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ouhdgbik.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3kdztbpkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvqhnvoa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3irdwkrbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zktvpdod.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3mdlyyqkm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3xfxgmjer.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3kguomirf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3aqlazoaz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jeechgia.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3gegmkbvq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3zmndudll.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ommtbvfw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ywxxkdfh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3obibbtym.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3kyzjjaej.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3qkvxktpz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3tpgygngx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3vfaqttoo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xiijzkdl.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3fhumyqcv.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3hcyjjhqa.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3uaijjhfg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3fqwmdbdj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3narndouf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jdplfrhk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wuifzwtk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3rknohiae.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gzfxhhdl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ouskfwsc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3tzgcybox.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3zytkhbet.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3lnpxjkjl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ukuyuwrb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3tnhrlmec.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3fhnvwgub.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3vhakdlbs.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3swvpzqhc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3dwbbgtzv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3xenlufew.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ycicdjkx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3zxovewub.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3lghkhdrt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3mrxlrsiy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3adhzokmu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3emyxknmk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3miycorqn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3vpewomhn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3jmaqqdpj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3zfaryuae.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3hbvqyboo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3qobmyiyy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xjcvzpzu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3trskqowh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3hnmdlrnz.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3jabvkfzq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3gonserjr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3zfztveoy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3cvhfwhfg.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3jgmzjtai.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3dqbcskje.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3djjfbkgz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xdmbiqlu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fpywtwul.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3mhddboct.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3zttqcvtd.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3yvhkldzz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3lhheokgk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3spimzmue.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3cwqeazpp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3heozntbo.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ohpeisnz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3xctirdna.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3xejvygio.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3hdkpgenm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3dtjrxkwc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3aoriwppl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3uklikebh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3obqpywwu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3hqymgllq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3bxmqkjxk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3vsbvimct.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3qdqfmkdw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3rbgtnafz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3omxcxtuk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3chgvgivh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3veyogrup.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3qrurukjx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ljmsbltu.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3eikeupce.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3rxsveoyn.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3hygszdxs.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3omfwkbsv.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3eajkgnvv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixxqtbfe.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3zhkiritn.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3simjbqth.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3efmpqach.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3gtvfwfuy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3aayeiltt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3reopjoxc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ydbsnvae.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3scpomakv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3qmrxopuj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3whpfwgei.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3rwpjpcon.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3zrxapaiz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pexlgbdi.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3rezgcdfg.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3zjjbppxa.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3piwkdsph.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3garqyaji.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3dtzodcei.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3hsqugchv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kydqsgob.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ohtravzz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3htyqkalp.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gzwgrhqj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3cwasvzyx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3kxotzhrg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jfaqmztw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3kfxzndzv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nnvnzzga.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3djtmbtln.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3blpladnt.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3uakbwrts.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3scoapkot.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3vzoxkumf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3lepcxxgq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3mjuozlgi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3mmbxlubq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3gulggdiq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3pcxhpden.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3xgcrrqqe.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ruqqufxs.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3nrtwobzm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3sjymmxca.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3afffkbjp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3jectlgbr.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3wevfkurc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3pfubgmws.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3kisypznv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3tnkbepec.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3pedihcqu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ixptamhg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xyasaeuu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mqwpnpdc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3vlmwswgo.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3vqzudnhw.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3oelhjmxp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3uybzewwz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3szlqfuve.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3opxssstq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wogdrjzj.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3rbxbqvof.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3smtkrvky.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3vxajdaso.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3rfdtrimf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3dxrptkvl.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ngbxgefl.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3qxkamhcm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3stbvncsy.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3namuxupd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3brxkqtjl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3sbgduwwj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3luywaxit.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3mgcjsegm.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3nrsuipek.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3wpepgmum.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3flqalkxw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3obihjdgh.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xpuujbww.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ibxttavx.html


<!-- 参考信息 -->