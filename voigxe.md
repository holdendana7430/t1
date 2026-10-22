代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdzkkwvh.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2kpjzznzl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2erifhyvz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ieodjhvk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dakwhfyc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2fdjjsnlt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2wnijipjc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2rmwdoxyl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ohjqyuud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrnbmjos.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2gjwvgcem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2prpnekgm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lsaausau.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nqaasacd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qjbfjljw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2jcaolrlv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ojdzutht.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bdkgtdbc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2czodzpyc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2irgmjhhq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2sutvnaky.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2lczadqoi.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2fptzjheu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tvllqsmx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2oyrhwuey.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gtipaewt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2sfhdmask.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mvjokniw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2tjxhwnmt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2kqblysoh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ycfgivrf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2lycqkhsc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2rokefagp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2zcpolsba.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ratfxvha.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qjlkzglc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2njghlkso.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rhxwiidu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2taizntbw.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2svjogymw.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2menenrhn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wvousziv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2snvyyynx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vlrbwvyc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2vwsmojdk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nocizpkg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qokhowhp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2oegythrs.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gesbpduk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2xxxhqzlr.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2pitkqptj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zlopwgbs.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2rddgbzij.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2pispgdft.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2mmxxxpwn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qxcnnpkd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2iuaihspb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2tkqyfrjn.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2sxtdxdmf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pcdgwixd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2uhzewdfl.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2yldxdlzp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2xpvqsjxg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jzwprmjy.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2axtbfjzg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2qmcqfyjw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2nfnppfdp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2imsraxev.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2yptrjmlv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2txcbsnyy.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2qinpjxaz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kfniejat.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dpuryokz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sdmcwvid.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2unmatoea.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ndjijwik.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pudinalc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2bmvoavei.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2trawtzcu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2vxoamkve.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2guwenoug.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2jmjaoajt.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qwbweavc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2idxdhtrj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ncpqfpsz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2iudsywxb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2tcjapwld.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2mqorkcsb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kaikdynf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2hjjgbygt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2jqrvtqvh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2pnmskvxd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gpmevlcd.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2kfhqzeuf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2oumprxnj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2aalqkrhv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nymjtohh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hgtmvyaa.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mmhvxkqf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdrpasow.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2njkeiyuc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2oowceibt.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2mrdadsib.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxwxuuqb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2imhrktgl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoavdzic.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2bjmceraj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ecdqjyhy.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kgcmwhnb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyydhzjj.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2chunytdn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2dmjtlbwu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2cfjgocxu.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2torvpzxq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lujeincz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2vqtdwssb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bwzixyef.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2trycpddb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dxuyeuwx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ejpawkce.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2bdpzaccv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jqozrudq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eypvjxma.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2itvzbkey.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2znletspc.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wuphmlsp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2bfvxirpy.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ydktjjlz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2hghdclba.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2igxqglxd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dvdoiotn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2wdmfzjaw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2kvjxpnhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ccjbtwsy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xnphrzci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oylrweik.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2jjxazjrd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2cbrlrzso.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2zvqufbzb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ieeexgzh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2cdgffios.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2lesrmmqv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2opfiomex.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2zxlbopdm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2tjhpedsp.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pwrpczgs.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2preylrtj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2spwanxbs.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2esukzovt.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2vabpycay.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2vfcrliop.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2gebleiaq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2mdzixrsm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2sydyndux.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2fsnnqfnj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2tbuyzbuh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2kssyjfrm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2kenmfnej.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2yjngfhmt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2suoqhdld.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2gofswjqr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2pvbwatoi.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2dstynttp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2vszfhvmd.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2qjxndifd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2cdyupteo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ytpzgtmx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ntuznyvq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2tmqlwgnq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2vctmozld.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ctrjjbsa.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gamybyxu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2sjchbxan.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2iqvddkqr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2gaonttrr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2lxicrhha.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2tjudcmtu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ehpbusxy.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2hjgfqgbb.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2yipbbdtd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2gpkmykqq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2zgdpnqyk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2mtozngbj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mvmuefok.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2simlwvhr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2pisbkafe.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2nygjbrro.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2aqeuqiqb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2lcvbnfyn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2lxhursbe.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2itwyvgve.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2epuutfsy.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2cmburtha.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2hoanvkpi.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2mpszuqze.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2xupzunpp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2cabexddf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2bfyicefk.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bsdxwmbq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2xonptyhd.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2dntdzbiq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2atztipjq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2lohmphuk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2aeajywvu.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2rbjztggw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ukksclbd.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jhrnwfnc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2mtafyvra.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2kqnbwhlk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ulpmnjsr.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2jkslklox.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2rlrpvhci.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2zqrjbyqc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2zvihkobs.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2whppgsfh.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vrtezzqi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2pumivavu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2zlabnhdq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2msjbmwig.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2vdnmnjzi.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2nlfxvtdf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2fzduawcq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2azdhpdrt.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2bwbfqiuj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2uvzpftcl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2czwckccs.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2kuiwmuls.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2gvtkjzcc.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ughyxbwy.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2zvkhbuoq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ncrvofki.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftmvamka.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2jgksmjuu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2pqosjdsr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2gyveukdx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gjzvnbzw.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ueqosyig.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2uiyjohhd.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2jeflbbep.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2timxzjer.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2lxwwlunp.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2dbigwkmu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ythecvrh.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2fhkgxxhe.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2whzwihsw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hoozvlqb.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lzyywbfm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2umnopwgp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tgtabpac.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2qwamzocj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2hwjwifbm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2huuxdenj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2cgrcyrzn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gfjdbdee.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2vhqduhzv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2utzbmsnt.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2gjqyhgpn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2nbgzjjyz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2pbrhlsnj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ncdmsvxm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2wdsbfopk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lhicbntk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2nnnqqbog.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2pkcbsbfg.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2aopxtlhg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2znwiokjh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2pctimskz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2bpxfrvpo.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2teueantx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2lkvzqizn.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2wwzmjuwt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ahvpkoyi.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2apyjzyhd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ttvohest.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2hsogmlby.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2zokjrblm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xeupyspb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2znapzpkh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2geyympor.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2rxrctzom.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2xoumbvmf.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2otcaxpmr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vvcidszk.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ifzyfkuh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2fiabedrf.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2lhjtiqni.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2cufvyoho.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ukkkvmoe.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2hxgttfsr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2majxmsvq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qdvojxpd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2kipbodxk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2yshagypt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ggxuyecz.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2asabjitk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ppzocuai.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2rhymsiwb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2jkwcsyxr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2nqkmgpjp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2tuchsfiv.html


<!-- 参考信息 -->