代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2rznekihl.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2wyqrclfi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2bupovmqf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2uqwqyfiu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2rfthytse.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ghqudlij.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2thstgbpx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2aofrvucz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zshzfwri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aaxmyfbd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2xcqwszzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nyuajpzn.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vxrfrhox.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wxkxobdh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2xmxurpwk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2lmjfgbct.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ujqcqxxc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2exwhxqdz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2voxzrtpn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2yqvdqjkx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gdwmzczh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2cwdxbofu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ptufjbcn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2egweszou.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2moqoocxh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ojbvjbny.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2fbnjqoxj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tbqosogk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2mchyzepp.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2avhywzlj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2evseawds.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jksnstfw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2bgrzfjhv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2exvigawb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2zcslgewd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zsqklbdu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2szyjphwo.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ajbieufh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2naardlsd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dxzpyvic.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2qzgehqow.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2csiujnvl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wsfvhgfr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uelremdu.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2phixldzm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2djgqahzl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rfxnzvmr.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2hxsizcky.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2mepxrspc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2akjhquhf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2tttsgimq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vdmxzgyw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2bdsezosz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2qnyipvne.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2zaoyhssa.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mfcenyac.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2znvclgoh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2puberbym.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2canmsnkl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bmbepxmu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2inrxbxoe.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2iqnocgey.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2jscdkwog.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2givbgnwp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2sjxjdcbq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2seniiigq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2kwbgbswl.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ghmljhsu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2mbuioiim.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2hzkippjb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2tvpcfijr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2zkcmpntz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pkfcrhsu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2carkshgm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2metovofg.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2pilpfpwg.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2diwlzqaf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2mzinnytx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2pfmqokih.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2hjnjbvun.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2yxwmkdld.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ltjhwmzr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cdnoruyt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2iseiuekm.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bnftrlks.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2vhlyeljs.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2biefvurm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2nwskkorz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rdhgefob.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2fffhsawp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2oijviqwj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2hnvgsvma.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sllkwhqn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ltrftvdu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2fvmlsolk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2kusnbmkp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dtqvsjpe.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2gljrtoxc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2slwckctf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2voaicgbk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2annacqnp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uybjlquj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2jllrxewu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ceybujwf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2afggqjnq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhlozvds.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2pijnwnal.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2yodcvfub.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2htdefged.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjpmqahj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wbkckavl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2gpyagrlv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2iypgkatv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2czzfvzqs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2emyrmqca.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2zeledwbe.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tbweykgl.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hlweblpl.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rwtroimw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wwmcfeba.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2eaxnbrhr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pbywmyde.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2fzzmidpy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2jarkbejx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2sbkryvyp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jfiboqpz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mxrxnxly.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2bzximrho.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nkbnuhwd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2zdhyevqi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nwkdsdlr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2lahczzap.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2njdxprsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rylpljkd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jsrcbztb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lxxceivg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2kuhtwwum.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2wtbffbbm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2gbmvvnlr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2xbkhtprf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2jpoltxnh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ifuzqiem.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2kyxglkcn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2pzlapfvz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2wivahqgm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ayfwgduy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2erdwwymw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2vfehtoip.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2inpuucif.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2hbygsiko.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2bujywxca.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2cbbyalgo.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2nyqezhqk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2kiiwqxhd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2zzrmdspc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2tbtdlryb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jpdejafg.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2qqmanzas.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2onbsysvq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qkehtbzv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2gwttnvek.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2dksgbyci.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2qovluncj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2jtwifver.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2xsqtzoba.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2rwuuifjb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2pdpefymu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2awifbgji.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2kgdybhzt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2otovcuho.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2kirmolnh.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hurodxig.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2yxyotadr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2svbaurho.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2qqyblxin.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2uxdxjpag.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2dxsfzadn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2fbkgvwmq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2dkrehwws.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2jqikjrpv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2twphwwvs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2cxekpgig.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2yuktiomi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yogjjuhx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2uyhjenvx.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2dhaxwuqn.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ndpmbroa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2jbssdost.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2riiojkho.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2syetxobp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2oqzmsjiy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2upmvotcw.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2shtxqmjs.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2trcnsqwu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2bqyrzsol.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2vpmtqyac.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2tncdxmqm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ueitjrcm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2hwyhunzx.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2jbpljnob.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2xcrowywa.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2hqjzhxqx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2vbsivmez.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2rsvirtic.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2nvrtylbz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2cprdqyeu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2gitjlzzn.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2jtpsvcqn.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2abckrbim.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2znpjcyxr.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2nsisjrhh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2yauhylxj.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2dahbzxuv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2hxqjczat.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2hbybgban.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ylnbziip.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2xddaduzt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2kcsmhpms.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ofholyep.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ocwoeimu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2dluizrso.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2uzqbsbka.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2yzixztdn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2wfcdwaux.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2urkcxumi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwjmgray.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2trzfmtaj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2jrnjujyu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2mztwgnbo.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2xncwuntl.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uyykpoud.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghshrkxi.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2skpzqwny.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ebkrtucl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2qbnjvhay.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhjzgohq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2vkegzbil.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2lvnmdiyc.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2nwsjtqem.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2slabidom.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2hpqoichv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2uuqkwdhy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2cpihnxnn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2qvhxguzr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2fkfahaqq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ixvuvtti.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2pbmjrvxf.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wgamtrmv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jlvzemfo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2fhkibdsz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2rciaftom.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2csgvhatn.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2hgryhoao.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fgzlxhpr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2tvicdquy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2xasuoifz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2jrxautyc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mktaualt.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2iatdmgdf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2qjawcidu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2kshgqnbx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2yzwoyejw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2mchfudnw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2fpnepjqb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2xibplgoy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vursnmzs.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2hgofefoy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wrrxiguy.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2gyugtinx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2lcypmhof.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2xqhbnxla.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ckbeoaxh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2mpdxpsta.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2cntpmwbj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2pnvwcvfl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2dfskclbu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2rqjdfolv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bruwqcgp.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2anoexkzo.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2zinnwalv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2acchjhhb.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2fdxquhrm.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ppoeoemt.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2axtqpywq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2bdjpzhua.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ydkiefkl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2pjvjzbad.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2phqnnbyb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2obboorro.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2wwlhsfju.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2bgfingsu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2hnxscvfh.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2sfwtxutm.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2xfodvxyb.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2unpbdtig.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2gzefgklv.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2kgepuwkv.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2tfinawid.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2xffpkaze.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2oxeflywz.html


<!-- 参考信息 -->