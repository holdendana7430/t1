代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqzltxhn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ruevartm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2huvtuthe.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2pgjijvxc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2pbwfhiud.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ymlmhmfm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2mrobcnlo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2idqrqvre.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vpxqnbci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ijekjqbf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vadsndmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttfuazmh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jdbkydvr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ihztysfq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vbhaccyg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2bsojhslr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2egiupgcr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ukrdbacu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2hmygnqkf.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2gtcnunao.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2isellkxy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2xkzyuegq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2okvdlapg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yrnjjexv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iunpcehl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2rcqtmwkm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ehbbwxsd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2joilqlkq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2xclcedjt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2tnmtcowp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2outshayv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2bkzizheq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2zaeacunq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2xnapmnqe.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ftdwniee.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gydqhhnm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2dujkkwqo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2fzicrmze.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2mvdpsunt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ihjwvzwn.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2dpvgpsvy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zudrberl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yxlxuqyx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nzbofdcc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ebnmkpdf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2qjtvppsd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2whwffkxf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2vldkvknx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2susymxud.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2nomcliex.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ttaudqqo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ttmlayha.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2mvavuunw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ufhjhdjf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2scaxqoxb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2atidnxrn.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2yencztue.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2joxzihpz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2twgauvmd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dnlybjeq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2pxafuqlz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2wnszdoht.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2yuboojsb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2abckcdsm.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2sbiuoehn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2kwyvsody.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bocpictb.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2apeqptbm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2pmajrrxx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xspiitzl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2hdydaopt.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2pjvdunme.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pgwidorz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2taprcovp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2waepwvud.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2uanxowyi.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lggubuoe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2udmninag.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xlixpeax.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2njmwhggh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ytzdssuw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jjfbbayw.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lqtkaxjq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2iiwettod.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xxvknmec.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2nrqlndis.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ddtsqlka.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2pjtgbodc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wwmvhphg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2dduvmsgg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2nxvbxhnz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2jnlonbqo.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ctyalytd.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2zmqnclvu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2flmkneck.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2evxojwnz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ggbbmcet.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2wauudkfz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2jlebpkll.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufsqczzi.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2avccqrsb.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuzucdvw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2iklohdor.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2nsglugyt.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ldwtgipw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2estblyal.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2rgajapjl.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2whlrprkx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2stmqitrk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xoaclyvh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gizgtdhi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2zdgjsjnm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2kxfignjd.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lddfaspt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fmneycnl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2fsozrucy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2anvitxqb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bztkoiel.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2uddkalkn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vwsysqwv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2zbqmyxcj.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vgdyznwg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2odmnkvzk.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2gjokkdbt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ntgxsahn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ztqpupyp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2cuyismqh.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ncwvmpth.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xojwykwq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2nrqgnqcp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xievkykr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2oqgekwbv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2wdmsyymt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yffmzxps.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2kxtfshjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghdgkbbg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2hhdojyse.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2jzneoppd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2pntsjhby.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hsyznlmr.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hrvtdyze.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2fvsnyxve.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2fidbxhba.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2bqghpysu.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2gmdknwvc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2egugsdiv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ehwryhrr.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2skkrxvrp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ufrrydpu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wbdtcycn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ddybzrwc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2wcuiyuaj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2zlqojlks.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2hbocikww.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ycpbscct.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2detrpqjz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wdxoraig.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uhtsnekn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2oapnjhid.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zrwsrfde.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2okiptkqb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2cnmerivl.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2amjocatr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xjjehafz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2mnzddvxr.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2nkgabjfu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2btxxossy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2mhllqwwt.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2uywfxemt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2unzztdtu.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2kbtpiruf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tbeealog.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2bxzplnyc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2idzxdosd.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2cqdnaruo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ilmoiqiw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2gkrfkifq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2srqzyqsm.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2dtaqrwxo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2mqqegcpn.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ceaigspb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2anqttouq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2bdodecsv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jgoedsdk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2msyzhoto.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2gxeuyyaj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2uydclozu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ryuxxdrc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2dkswrvqt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2snhxvtci.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2nvtpyzru.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2cdgqjptc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2eopkolbt.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ntrxwgeg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2zlheiexc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2vepujcwb.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2pfmtazix.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wrbozmnb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ebejyszr.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2mmxotruv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2pottxlif.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2iaywdqcb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2qpgctjaj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2vtaedqnm.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2pyxgcnoh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2bnmvqhyv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2sywestfx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2rhmykqqr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2fjvesxot.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2uxwaalst.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2oiamgwcs.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2cxdpazdi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2xwvysdor.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2tqatkfoc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2cengatcy.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lmaqvgew.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2syqtjmgo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2egztnpcu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ysufxotz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2tidrqruc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dswgubxn.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2tcupbxcj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2sxgtjvhv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2zslkpiyg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2tgyjnjjm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wnvmgxnm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2dekqlepc.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ihlfeatc.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2xgfhljrm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ukngglef.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2peqvtgdm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2efuvajdt.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ywfxkzpg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2rhanovpp.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2xznhqndz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2gxnzkaby.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2stmhwnyi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2shxdhvgb.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vlvlmdkh.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2upktogzx.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2wtneedwv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2rlyhdreh.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2xbtrdrrc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2pqzcuegx.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wgijyajs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2eifvkqch.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bwcohmph.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bzhfmomc.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lepbceiu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2zodekvri.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2hhxlcyxv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2sztuxxwv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2dlhtbhor.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vzwracyz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2uihsebhx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lgrkawse.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2iusmgour.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ydsicrdl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ffanvofg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ecxvtprl.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2nfawtvlj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2nulxhwpn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nicaqrxd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ofafpemm.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ufgyzabs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2znqixuhe.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2dqjlmeul.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rwjynvjo.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2svkgjmpc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ttidtoyw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2qouzewlw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2cbtyzqqx.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ukgysieh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ibhivwdm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2wiamuesy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2nvbpxluu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2krxeviug.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ngtlmwpx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2lyktsunu.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2wljznojb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2etzhplfn.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2rowvaimg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2thqyusry.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2zzdsmvia.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2gjdtocjj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2yetdpbey.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2bgjfuhpn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2bxlsgyfd.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2uazniklw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2sopzcjnj.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vobjfwbr.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2berggjtf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2aamvvwuo.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2cipkchvc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2mbwspwop.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2zfznyqul.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2kwkqjqvs.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2icoxrkae.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2wlkudjho.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2hohqxxxw.html


<!-- 参考信息 -->