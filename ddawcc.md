代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2oysfwfaq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2vdfeumam.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2lamudley.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2lwxucluo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mszoiqod.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2fcltwqgu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2rkesmkrx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2nlwvaqbh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vosbqcwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhrggqll.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2aamrpxdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ycrxqmut.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mqmddoea.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2iebfqyrp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dekizybg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2zjghndcn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2tghosfpq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xjxmzqiz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2zuqmyanx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2kbcozeay.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wzjbmnlr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2dvagacle.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kuhtdufe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nilnvznn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uevmzytx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xktfmpid.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2qqtxhegy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2henqlxfm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2crzbhtfh.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2hxrizpir.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2sefpohth.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2omzejqqi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ceisuhph.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jahbcrnj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2kmdzowup.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2haiyfwuz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2euviruwn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2utxjnqhy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2etbewboa.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dfzdrkwa.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2lkfbgmqo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2olgrcglb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kskexfeb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nhhloznf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2gckrepti.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ligteqwr.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xzelcirz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2yudixvmo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zgctxzkv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2smulsjvj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2nmuonfaa.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rjxvfaos.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lfptzdnl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2tfxbmzfq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2trlmdosl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2eplmcefb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dxwsbczo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yxwcdmal.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2wcukkknw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2brouguvd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2sffmoxfb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2imyqcebn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2mpulzafd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rwmizqvv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2qydkwlli.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ilxjxugj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2trfdubqp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2kuokqdbl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2itghekyy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bigjqfwm.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2npfuqgbw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2giiznjip.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2azyqeifz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jrdotugw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ecjazmuk.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dhooufba.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2phqierkp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2zzozqgor.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2raxbcbhi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ufzwtlul.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2hbdjlmep.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2efewwmnv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2evlwjtwb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2catxntpt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bwzqiwii.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2zauaxyxk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qgjzjgil.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2khuimfsa.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gbvafbyv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2pddxacjx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2yezockho.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2tuofvrnd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xuqglrzx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kpgvlugv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2kaynozxp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2bycefozp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hibomzep.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2mfovgljn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kknlucuk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2astjmxju.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2srfvpmvk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yczenrhu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2hzidxofb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwhxgjkp.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2mxjtvpco.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjhiywiw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2lamafzua.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2pkzieqih.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wsditpya.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2egezvqco.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vyfeqdfa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2bjznbumv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kauoasnw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nyerikol.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ixdlujul.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2qxniinls.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2bjfepsaa.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zdgpgrfv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ztgcwucy.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2feyfdgtc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2mrretvmq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vnnkxdmz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vwyzkznb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2srrwqijr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tpwovifp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rygyxlcg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2kbkbwgao.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2vjtxsahj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ouokxfgo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zxxmylty.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vbtguqro.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2xiqgficv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2sujgjfdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nvlzdvrh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bhboypuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irfuxizo.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2vzsjptco.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2dfoidijl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2htspcvhv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2odiiozbq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2adxpwkuc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2obwndubp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2nntsimey.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2nyutcwzy.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2kbtewwhy.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2teziwkkd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2fvvcgzux.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2tyfspzxu.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ggumqkti.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2dndpakna.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2znjxdent.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2hofjwhif.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2hyqzcdes.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2trhkaxdf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2nazivacl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2glrqqcvc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2cdjxldgi.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2dxbzhruo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2wirbcqwq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qxuxqlpw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2lhkeihko.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2tvcbwmlc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2csuhrymf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2aekxbqgu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2csjwdckg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2qhqsxiga.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ywxapvge.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2miwfzkbl.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2jbyjehyz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2pvcekkig.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2hffaerxi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rsmyybvu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2bakmqxmi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2oqzdpzuz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2zeomhegz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2vsrikljl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2hssbbnqg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2docdrrzv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2gyudaaxs.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2sjcvptrq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ugtxukhi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2rvcawtfz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2crkigghb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yduyffwj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2dcadndxc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2yqxxirwx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2fsuwzzgg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2etpqwgqh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2amxbujsj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2yphdsqwy.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ellbxdvh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2mpodtpjs.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2mrpenqpc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ufsbxthq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2gwlbuofa.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lylaciap.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ovzgqkai.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2wyisnzei.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2aronwpug.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2cjotbbsa.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2hpjbavxm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2inkkutle.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2shkwidjx.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2eghiegoi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2myskoqhp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ulpmiwzh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2tfbngmxa.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2dqlljbgk.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2fmvyzovi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2tvfhtejw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2bdnzlrhe.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2kdtydfra.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2bucwbmts.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2adnwsozm.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2krmswyly.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2frjbpjew.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2lombxcvu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2abstjxim.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2vwphfazp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2abnxetru.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2hqqxvrja.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2pihdpype.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2teartkcg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2nifufedg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2fljjobgs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiddrnro.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2bwqhzvhn.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ovcslzvg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ckhizzox.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ccizzhty.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ohpsyfrk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayjpsxtf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2idhghobf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2sahrcgte.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2mbdgqlhy.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qncjhbab.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2pwlzuymg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2xncksihf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ttbowyjg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2gbuuioea.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ecfhwxpd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ybmmkkct.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2kihagwez.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2mzkobicm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2kjpevqwp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2oksakfxk.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wqlkwuhu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wedvylki.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xlrhpsbd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ofhpghms.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2uwdmuwrx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jkdfohyu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2sygupnjy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2efwxtyax.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2jfkotift.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2uiyiqgex.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2mwpiqvlm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2qlwtmdue.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2nyepdole.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2veqegqll.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ldrjtask.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2blvbnkky.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rihkjaos.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ofllatkc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2cihvtxhj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pmspgewk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2qszglrus.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ypkkcfdg.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ffttriag.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2tljdburz.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2oucfhqmt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ibywvgzh.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2dyozxwlz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2losnwdqm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2uplqwwng.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2veszlhqe.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2btyixuna.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2msztncxu.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2deyhmscn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2bdxbisky.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2smkfvouu.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ezundyaw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ryadzsgq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jtxolwgs.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2lcjkqufs.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2lpauncqd.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2fckeenim.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2pqrruzor.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2gnsacssy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2szfabcsv.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ugpvkrzr.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2sbdtmfuq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2uvxdbncc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2glnptkrp.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2goagdyof.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ezglbhea.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2brcuaqed.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ppxsxhmb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2nkrukvbv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2huvnefjn.html


<!-- 参考信息 -->