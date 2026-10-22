代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2czyhfolr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2usjfanqk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2dpmjftbu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2xphcrurr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mjltxufc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzukpwnd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2sqhznwux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqaqvake.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rxshsmqi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2odffdbrf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2owngxhib.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ksvukrvi.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2uconghzs.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2oekjhikm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ymcyrvrq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xlxczxnd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2mbsvlqbm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ujexosej.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ofkonzth.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yubxoqqb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2znoofkfr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ymylcekc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2bfubqvnm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2oaprzmrf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2iyxhvibe.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2uqepxric.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ntpmffnm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2khpyzmmz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2qbtfqsst.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2phabafdz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2agdppoue.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2expbihvo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2nfhiqrss.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ojbnkjcp.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2krniiyxr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qjsraqte.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2fdaelcmj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2fxvphtfg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qcwqtxof.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2maxplroo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2euqhayer.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2qecgqmyq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2chcysbyb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2kengpxct.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2jsjmojyo.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2vixrwjaz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2aawakree.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2pdvsonya.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rjzrbjzi.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rkiksttu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2oqpjdgde.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2yxwmttjh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2bdostkvz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zbhnjljm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2jfrqskze.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2glfwwpmz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2envkjduu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2htpjhdpz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2iwdldibs.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2utktjdmr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2rsplqepq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2dgtnrlln.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2vyrbndhh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2xbuvtfvz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2lfwkxphg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jlsteddq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2glfsrwcc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wspledad.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wukcxkqh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xewefmdh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2lflnxhbz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2spgchpwj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2abdfrmtg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2tcxdfjhp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2itnxxafx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2vxzsmuwe.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2pwloyuka.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2dgjrhuru.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2oykdwtsr.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ztvjoits.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xrnogspp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2klbtugay.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ocegayod.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2unbiaaff.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qtfrkzis.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ydqxsoie.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2fmzkgcwr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vqxhzusu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kosxxqav.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2rcvvjqws.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2mtgdzgru.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2sfvrxdys.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2awzuabsm.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2aqwzerhl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fepcpbss.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezaqjckb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nrjvxjsz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2rmjkhugn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2tvromlfb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2poqplcjc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2zmrwyapx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2gnydkhac.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dfrvqrow.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2frhvjxpw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2wwsqqwpb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bcxuuocn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rodqaufu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2kwyaywyp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2zndxhkhf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2prwyxgpv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wrtppoxr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qmrikzso.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ejfinlpm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xboysynd.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nmzifabc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ojwhxqqt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2exosjvpt.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yeqdcdwo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2utwwqrhf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2yejjaese.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ddvnbpis.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2noztpvxg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2cgyggjug.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2irlyisnb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2tjwlolsp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2epspbhvd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ubuqmwzg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2pntqsthu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2xjnwdaqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jdzvgsyg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rhkxysqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwatgdau.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qhxsstcy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2kjzevfth.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ckedumzt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2rewftplj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2wrjcwmmx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ridvarxq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2vdrrnzin.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2uoqwppsg.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2bvlpmuct.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dhytewdm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2zqudypng.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2jprzbzfk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2pjiuiqim.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2xmnuycma.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2cekctkrl.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2jcmmehge.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ezboflbx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ipavyymk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2bgzqeels.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2pvqhotij.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hrlqiyji.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2vuwbgtgd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2xvivldaj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ddaznkwg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ggqnuyxv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2qgfhdgrm.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2hjpsyxkd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2xiwjwpiz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2nrhtcmxs.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2npfqffrd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2dmpwzpjt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wnuwegor.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2irbsrbod.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2kiibhiza.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2aevnwpsp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qhvoukqg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2wbljrvio.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2tjfvaxfe.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ilhzoexs.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ecqwesvs.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2iyflslun.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2yunnlyfz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2pttqxisn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2bunpjrxw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2oqcyadkb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2mscaeavw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2jneqgbih.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2azwgwttt.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2dfpznfoj.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2sspgtywb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2wdbtnihj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2uersxmla.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2lwloncny.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2byadstwi.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2wmatylfp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ftsiybil.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2wjgjmhil.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2whxlsqvn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2lcluioyj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2gpmohhub.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2kzlhldsp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2sussqmwc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2npnykaua.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2vfwdxsav.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2mellnggq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ybxuqeck.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2xioticlp.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2dqbkftho.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2jgbnwmxr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2cnqalhrf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xqqwuqdy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2fqolfwuf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2fngvicnn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2cvqtlkap.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2fomfajbt.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2cmsdqcyc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2lutzjkxa.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2qsnprnid.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2gltmaiaa.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2hppafwet.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2wnfbnkdv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2cuszpttd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2vmtnyrmj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ezxnlmfy.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2emahigsf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2zwtjibhh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2yhzdksng.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2pdgajzjf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2yrbhrntb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pglntszz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2anydfvpm.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2iuuxgaiw.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2uyduhogf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2qixedvjb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2citoptpw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ysgvukch.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ldmxezlh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2pdoxdycv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2dhmdzrlh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2voihxwtg.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2zzbhtxsf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2vgzdxepw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2auohvljv.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2djxdsrpb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2sdmjpxyv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2eobwkail.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2iorpgwxe.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2yslkjcqh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ombuabxp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wbwtnndh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bdbxiwyq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nhwnxexg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wjfyxpxh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2abakkjgg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ojubbfsr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oyhtnlwx.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2lkowmwpl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qfgrgegl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2xjvyosou.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2uyerxvjz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ocmlwhtb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kimwcmey.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2vclotkgs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gozftgir.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2sjvbyctd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2bbsvmlie.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sdpznbdc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2bdnmgihv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2lxyuqojs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2juriwnhw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ktqjtgzb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zlzackwr.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2tknjkbct.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ighymxls.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2dyekcazj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2vkttntwd.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2mntpdkzi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2inliwiba.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2tgbwafqm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ucdgwzgm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2akahqgiz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2griaprun.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ivkoljmj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2rwgrgwwn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ttqyecqu.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2rlkcwraw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jesaaipj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2jrwepcma.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2rqtogezj.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2puqoelfx.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2jcjgzyfk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2rgsdlxyl.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2mvohyewv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2orxzncpy.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2nqghlofs.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2wesgobst.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2rgrbbics.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2covxfhez.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2cdxnybth.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2whjsozzt.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2lozwgdxo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2gfzyatza.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ogzhxytv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2mfozybkp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2sugesgtz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gandwqaj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2oknctqbe.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2bqiluiqx.html


<!-- 参考信息 -->