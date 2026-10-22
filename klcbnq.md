代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkpyjnnj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2bwnywkrg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2gcukxuoe.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qnxtitmo.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2lpzjlzqw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ojfyodck.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2crodnwny.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ajfcyubn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dvpcycta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfmiiwup.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ueruhczi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqmpukmk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2inrjhfmy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rwfgwqcr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2phyhpvcr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2nlhoejyp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2kvpqgrpn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jjhutbaq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2upczrgav.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2obmvxaia.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2yetrdcyi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2jonsaqav.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2mbyytnlb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ahcdpgzb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yaindohl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2topwjrgb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xxpkprtw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ywiaebnu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ktgaflem.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2sdcgesmz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2heoykxoj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2genbwdpt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2jqgnycvh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lnlzqhvm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2wefuhcuz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cpnyyqdb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2esfnpxos.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xuwmggzr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dsijbwnf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gjrgncyd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2mtrrycve.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2goxgqtex.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yxwjygry.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lmafhmfi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2zalhyahc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2tasomnfo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2blvlcjqk.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2pquerqdc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2gbjthjva.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2yowfdlgb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2hounkmpm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vlowdvnn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ctflghdw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2emtjbxlp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2zwkimust.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ivjgdnia.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2pgzjighp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pcmoaaeo.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bmkebvqd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uemmcfdj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2wlechito.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ogslqvmx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2fqtgawjl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ktjtkela.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2wabccpmm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2rmzegfue.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2wwlxcggr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2falnoqab.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2oqicnnis.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2clygxeoe.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2mohdxtmy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2lxwbkwsk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gjlnpccf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nuhyuekp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2crnsdnnl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2qlffzzeu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2iqepyqcm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2yciuvxwt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2awwsaevm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2vfmmedet.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ipxlerjm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fuogkatk.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nkvyyptl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2zhebadyi.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qqziuqts.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ocunfvxu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2hrmtiybn.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2avjtkqjg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2esvybeif.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mihowdgx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2tehluogc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2xiyteakn.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kdojfwsj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kmiobiny.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rtcdzoku.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2palssfpw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jausyfwc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2eguwqxfd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2nzuujime.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzdtohsm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uehhgcln.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmdsblty.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2zqqxknzu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2dszanufw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2loujzazd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2fsodeikl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2akbdsdjw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2lggithuf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lcwgcpvw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kavsowtz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tzkplfhd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ktqyahxx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2eobsrony.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lqcvbmek.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nyipcdxe.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2dyyidlco.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2qqkvnfyb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ijbnfehw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vthtrgab.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hhyjavaf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dngopqrr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gzndjlrd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2wworkdqc.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2orqvvnpr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2kttimrly.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uwhsiekl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vyqevlzr.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2moozebus.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2nvlolqnr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fcixbubm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2shwyzcxz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2bgyesffz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2txnitbme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmpkldca.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pthaorbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwlgtaqe.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2tkjzfzee.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2puqvmhfu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2tnksckbt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2knhfnivx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ijsudjal.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2zwstndto.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2oyzjgsxo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2gttvupdh.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2svhinfci.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ifcgxjth.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2yxqrqatw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2dthjhiuu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2quaqejqg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2nvayzvwk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2yygrhrjv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2hqlwbrpw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2qreqayvi.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2rwkcfubd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2mzgoeyai.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2gtqvmmdb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qcrspiup.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2rpqcvivk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ubvvkwle.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2lfzeeohi.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2usbdogxy.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2yfuegegp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2bfjtdlsc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2lppfrzfw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jpiyfqsc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2goqyjncd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2lkftdmqj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2kjztfuax.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2yhvnjzwd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2xbfpirmf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2czsaduhg.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wvrxrwnc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2zddikldf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ymvuynpa.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2nxjpoeyc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2tydepgns.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2sstefbdw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2pznregzp.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2vvlgndua.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2vseljymu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ntusuost.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2zpcpsaim.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2bedewtxt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2feaopmcz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2jytmpsfz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2occqcybb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2pyswnlgg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2jxdonkid.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2bkpdztiz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2xmqknhiy.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2jeqnnmbm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2beacdeyd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2hucwqqpv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2isshezfs.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2azaxikbd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2npuzbxht.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2enokxhor.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2hatbdihp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2vzzxnudo.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2nnirdnyp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2mvmwgepn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2hrgzlprs.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2wnszxuab.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2lxwnasvk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2cpwzpduc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2uevnmvwj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fykeqweo.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2zzpqjicf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2dihwkpip.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2tmewwdko.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2wkefjrqx.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2wqulncar.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2yudukmhc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2pxjlbfgf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2sqwgkkhl.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2hkxebknr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2tlwuqalm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2cqmllals.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2titqslxc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2sllzormy.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2zmbpzjuh.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2yrlgyuua.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ufpkjloi.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ciyrmjix.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2urzztmpa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwszavys.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2sdxcrajs.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2qksvrrfk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2tlttxjjq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2dorqlazg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ltwjgfcl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucnhqbpt.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2vvkyazlf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2fxhsdbrs.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2rdozkgih.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2polvjvme.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2caqtdfuv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2mtifhypv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dljsmkos.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zrywptzb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2pexoikaz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2jtzfxdoq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2qjpaehgo.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2nwjobsez.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2xuvjvoxu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wsgsysmo.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2opizwnqe.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2twbttmwz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bcbkzgmv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2xvxnuhkj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2izkjrzaf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ojfgwoms.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2rhzwkpqh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2lotjuuyc.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2kpyiockl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2kqfuzrfk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2mxdvjnhy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2adbyencb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2pskelrdk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gwtlakek.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ipbaobuf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2lgoqlbuv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2souktpbg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2zfjkkzrb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ywngcicm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2byqurwjl.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2lsoyggrc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2xezkigjf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2chyshjcj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2cyuznqzt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2eypxkwco.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2hfinufck.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2hzlwcfka.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2hzctwrwa.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2xbqqkyrm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2oguxukal.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ybqnarzp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jhgjpuvn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2mfqwijon.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2bigodivl.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2lqahiptb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2spypiqjq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qumccvvy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2fvojzxog.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2vhqvxkbl.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2dvjvjtko.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2sfewhbtj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ljescjxv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2nqogjvig.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2xxbszeem.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hsgtuprr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2frbbucri.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2kbmqcufr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ivmctifs.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ujxjekwt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2bhottstj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2lwmsuwhz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2zcvtipmg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ajaujnoe.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2yvgzkaoc.html


<!-- 参考信息 -->