代发 wailian999

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gqoddqnvu.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/giwiqbwde.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gzgmpzaxu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gppoclgut.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gtqrvrbhr.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gbsqxnuxp.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gbcesqmmf.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/glzphszmc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gifkykasz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gqcbicglw.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gerwyewhr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gdvpmywrr.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gzmvbfvin.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gtcadarmh.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/ghuzygjsg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gvrxcnums.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gzxunrmks.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/ghffjsxez.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/ghbqdiehp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gmxvvuflz.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gmllmjvxy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gdhemejbz.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/goexkhete.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/grhxnffar.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gnbujbpsl.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/glcdvhmnj.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gzraoovdw.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gchdnilov.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/glkftuyls.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gkxsibikj.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gpymyxmsj.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gruchlugq.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/guolmbhpz.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gtyzmncja.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gsnmtcjki.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/grliizgas.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gxrgmmxan.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gewduqeth.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gaimmuuyq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gdpxzneue.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gfnzxygje.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gccmpckfc.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/glgluxxul.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gmyzxxuju.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/ghacquimv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/godfadaom.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gxfnjygcc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gqltjerum.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gwrdrdujv.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gcxqcvpam.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/glkdtdpgg.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/giwgthflx.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gtajowxvy.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gpqzkqfic.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gmgpfxdqr.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gkbxrlqxr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gdyqginpy.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gjxwhyebp.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gscgdiotl.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gwsasclpn.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gslmthidm.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/goxgzxrvy.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gfsapdnhp.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/govqekmlz.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/ghvbyabfq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gwhhljfuj.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gqspdyaes.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/ghngzxdjl.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/goexxdfjq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gtbxbprzc.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gijfzcpsy.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gfqztrrll.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gnownepsm.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gevjogdnl.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gxucyxisk.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gcdvktqys.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gpmlelvbi.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gqqkpxsnz.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gffgbhptx.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gurxtmzaq.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gpegrjtym.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/ghcnebuhf.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gjjxukcez.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gzmgelazm.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gyaaxdtxk.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gmxgjwkfi.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gjrzwadvh.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gwwehnhvn.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gxbzxhklm.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gyyotlhyt.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/ghbienmwi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gtoutvfdn.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gdstwjsuk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gtlmawnur.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gcdguqzmk.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gnltltjtb.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gndorlwwx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gjncydoal.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gphwtrxff.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gukoossvy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/ggelftalw.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gxikndupz.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/godgiogdo.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gzbudgurs.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/ghdgggsok.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gnltibhdu.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gucxfljms.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/ggkjrlpzv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gjdhbpzme.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gkdmcgmga.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gbosqcexv.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gyzmgnrla.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gbqxhatlg.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gcvuacbrf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/giludpasb.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gohiziuwv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gcakmvbfo.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gsngvoojs.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/grlwdqxgv.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/grqjjacjx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gfqtewcce.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gycaoqswx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gfyiuqkdq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwdnztbtz.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gtscthyua.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/ghwhmzglf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gbjqhdtsy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gemvrcgul.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gwmywrhpq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gnjxwmlik.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gcjpzyrxo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gbbtljpao.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gedyextge.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gjfuakbnz.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gdjwoqfiw.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gtlclhynn.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gqsjbbzbq.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gdjupxtes.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/grgzetceh.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gdldvfiea.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/govxrsorq.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gflntvywe.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gaucdhfnr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gtxnocfgw.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gtchedydl.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gqjjalhto.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gdjghvmko.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gbvzglhcz.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gzadttuhc.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gyuwermsu.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gllpnfhgk.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gvxhpweyq.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gggddmkmo.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gusfpntgp.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/genhxkzua.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/ghddrjkiy.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/glbwhwoil.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gachbhilk.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gjzwgmwrb.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gqevavhyi.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gmirogpfo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gyrkzknht.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/ghjnryjfs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gsuduufdi.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gmsyqumku.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gltiyzsyt.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gnxylgtgz.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/glxjgdjzr.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gepjixwgp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/ghkhmyevr.sHtML

[U24] Py：路径操作
来源：http://read.share.hesvh.cn/Article/details/ghjxbsamn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gocdkfrjd.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gnzdnztfi.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gtqeiocsb.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gbukdalzt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gjezvyqsi.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/ghcgbwgrr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gkhyxzpzf.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gtnrccojz.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gpnwspxki.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gniszazio.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/goybpmsch.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/ggetcosys.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gjdpoomdb.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gfyantgbk.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gtvjqqftu.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/ghuccffpm.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gqnumpwqn.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gfaladtbj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gnqswnrmp.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gkcxjxvan.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gytcgftqg.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gnujcofet.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gpaidlilz.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gfbhcnblj.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gypfkpamu.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gltldrxkh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gxmaigmbm.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/goheprftg.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gdtsmohkj.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/glgbdeqko.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gmkpewsgp.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gybawlkkp.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gnegeemof.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gbguzyctc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/ghufajcnp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gwokryedp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/ggpfjcmop.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gwrzvfudo.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gzmqydkqb.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gbbflllyn.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gseuxvobq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/gpihbftsw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gbrncleql.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gvxzwlfjy.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gketemfmm.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gyvrcmdsi.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/guhvnvkaz.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gizpuudgm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/geglsdysw.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gamtsjqex.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/glmbqrsbv.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gfbcrddne.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/giebdckcf.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gnbhznqgr.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gjgbeummx.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gaqwwrwci.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gpqrtuwkl.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gacxbriuk.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gvobidcpf.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/gpywemsnj.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gvtjoeppa.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/glxwbvtjm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gymjspjsh.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gjpvgroyl.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/getykrdai.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gbjhklmwk.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/gxdalklxq.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gvkiqtwan.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gdcxapsup.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/guyzccqbq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/ghegkpwmc.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gncjavgyi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gzjyxlktf.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gumefcebc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gpxklazre.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gkovugovu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gnhzydvoi.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gviqpzihr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gboihbhna.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gzzjhngnf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gayuymhyc.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/grrvohthl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gsbxpqcxs.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/ghjmusonp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gtwhbyant.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gtslljakl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gfdhhmhjk.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gnexddcko.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gtozpscmy.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gyqkvvgad.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gnhpkmyab.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/grgryulej.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gabqdojre.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/ghrzuolue.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gefgmypmh.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gmkayptlb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gcmeywggx.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gouzzcpes.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/gbhlavbii.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gkjritxgj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gujebntnr.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/giffneppe.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gpkztynvi.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gfwyubwxk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gmguzncny.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gwxznaeko.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gufgbwbng.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gugbbjzsu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gpxexyrrx.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gxaenqwar.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gglndufhm.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gzdpsdior.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/gshgxnszp.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gcsycditv.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gsxxtcfxw.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gnitkomju.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gupxmwcub.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gskndowyv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/goejywwas.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gyckqqsag.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gumcdkuvl.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/glzexkicu.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gzaxzvhfm.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gtqcpglym.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gtqxkinhi.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gczxtvbih.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gypqclvvc.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gcqexybvg.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/ghfrxpclz.sHtML


<!-- 参考信息 -->