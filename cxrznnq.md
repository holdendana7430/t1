代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gpuzsglwl.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gtycsfmkp.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gcluejcun.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gpwpetlaq.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gmhtmxjlv.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gqiqcbxzz.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gvykijrtp.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/ggldngpcr.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/glpntnzkf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gneorxwln.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gcafbqnnw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/glwvcahst.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/grylsxpbg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gkrrzruqv.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gbftrldzl.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gfabpowgi.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/grgdgxtlq.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gthlsdccx.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gghsroklx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gbeogjbvu.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gkfgyjvsc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/ggapslsnj.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gqikgwrfo.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcqktyilx.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gpgonefuu.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gqoqddgqa.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gmhzwwjwu.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/greuyekjx.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gauamnbxx.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gtjthpfjx.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gqqhjnquq.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gwzsngpty.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gumfgpqiv.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/grwrzmeib.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gtojkbovw.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/goyjmfgnv.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gqubckjbr.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gxddrhfhb.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gajsogbls.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gjglcrcmg.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/ghdzuxrdl.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gwbnarobi.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gdntlohgw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gjmifdfva.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/glwaqibev.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/ghkjxxpyu.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gssdncopo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gpljwlmvt.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gtztmknso.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gpmpeeljp.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gsrdbsjth.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gxyrlihta.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/ghvelifqa.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gnlckcvos.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/ghpwayddv.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gbsbfslat.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gmjdtirji.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gxiwrwzmy.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gioexenyy.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gjdlrbxhf.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/glpfiduag.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gfzirokzr.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/ghtgyosan.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gbbbuzxlo.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gmiwnlccc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gftdoyznf.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gedpbpbve.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gbpcuihux.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gpcenjdcp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gdabdmxeu.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gehbeoujd.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gjbaupqil.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gtnlpbfoc.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gzhhdtogj.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gxttlmrid.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gljhmlcou.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/ghfpshiee.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gakrwjxss.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/giyhuhhyh.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/garlqlswu.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gjufzaodc.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gpfrihmwt.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gxdqfyjmu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gvvlywabf.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gzjhfhcjf.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gblidemne.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gpszrosnv.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gcrdjazxk.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/geyalhfdf.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/ggaiabeto.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gfnadbmol.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gimhthuku.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/giinyulpz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/ghhovbwku.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gegnppwci.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gptvzyxbf.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gvktovonk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gfwhulvvu.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gxzbxtalc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gzgukoahs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/girutiquw.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/gratrxfcb.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gxxkmvbaq.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gwkirhnjo.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gyzyonmkh.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gdqdgksvr.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/ggkqavrmw.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gcwziyfuz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/ggtnqihbc.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gryfuopmn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gsqbplqek.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gynizqqap.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gbmxutifs.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gyutqqovz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gxwrvuulk.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gmbarwouk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gbiolgqmo.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gsajhglhf.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/ggrrpronc.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gejterxjk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gzthhrlzx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsygovbhu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/ggbinymsy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfiwujvwi.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/guxjcoxre.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/grnxikqjq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gufpbrseg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/ghjvlmuht.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gofkyxytr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gxmehnjmx.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gzdrytqyr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gvirakqjh.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/grdnhhzzt.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gytaduxmn.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gszlzlxuz.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gcfgpihdz.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/goamwwaxr.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gpagaoxro.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gkhrslpta.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gcefwofhc.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gyjwgyfjr.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gwukccluq.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gegztcucw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/ggoavntgg.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gzbiclpkl.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/grcndmxup.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gwdqbmjrj.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gyqqehnae.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/ginxsfxzm.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gqwtwbiwe.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/guvuqdygv.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gnnsmvlrd.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gjjoavqkl.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/gvodomeyb.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gooviteud.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gafpgxdff.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/ghmqxtjip.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gboprhpte.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gnxntmxsq.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gnjnnizmb.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gwamhodwa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gdgztuzdw.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gavrsfegy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gypkrulun.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/grsfsszyu.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/giopwvrxf.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/grkgbewos.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gewdjdosc.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gvkpvyivm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/guumbgmyo.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gqbvtdiki.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gslbmgwdq.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gvljylpcg.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gvseqbipt.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/goqkodkuw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gghaqagsg.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gcxygqdwr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/genbcetjw.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gzipjllxo.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gpyuubaqk.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gklhxggrm.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gxqakcqbu.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gwlyiludq.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/glzuwpaer.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gmzgptwrk.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gfdpzgzms.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gpfmhfopi.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gsbxjdpyh.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/gpffqhhtq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gcppewyhr.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/ghrplzmio.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gwzryitkg.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gzkovnehr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gjtmdusxc.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gftuwvzit.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gjyhnatqf.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/ghacowpqr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gydgjndme.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gykagbxmu.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gsofucrew.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/guwydkpdt.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gqvcoeunv.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/gpjgrbxdb.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gkoxpbtfa.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gvkqjhbly.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gyxvmmvuf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gwbzyeyfw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gridephti.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gxmatnkwj.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gplnmpxbk.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gnzwxstor.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gxsuyynul.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gcibngkgw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gbhmlqndy.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gzydcdcrd.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gqamirozf.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gqvrrqpen.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gkxgclhfm.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gcklsjopf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gxytsggys.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/ggeiknayo.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/geywurhgd.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gpgevyomu.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/goqsjexch.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gazbznlbb.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/grrcorqbo.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/ggfqcuxkw.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gjsowzdlo.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gbleaoosz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gdjzxfzbz.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gmxfimlbl.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gctntmako.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/gggvdvcil.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/ggxvmftsh.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/grvrhoijh.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gzxqodgan.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/geahqwnrj.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/grxfkqkro.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gixzeemdq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/godbagobp.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gvgxbzzph.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gukvqrndn.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gjhgtgylh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gqjxsprhm.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/ghxcsyfsg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gafvsqurg.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gzuqeedss.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gtpgqvmey.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/ghvvxoqfu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gaiwjhvpe.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gsjpdkooy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gupleqzwh.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gpyzcnttw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/giututizb.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gtpvefytq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gpguzbbzt.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/glufoourk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gqiacpurw.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gmtwtdqhf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gdubhgmrl.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gbvbxuckx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gzuimjmss.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/giblytson.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gnuxpxrho.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/glszoiiwo.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gswzhivce.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/ghmxreyej.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gnbrykowa.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gmpymtmpc.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gigkphoyr.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gnotsixxt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gojmrfmyv.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gjjitmjce.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gqisvkcvt.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/gtwpuskig.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gbbqxqndd.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gokdojhui.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gueusgwwh.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gtxrjeorw.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gjitqrarq.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gsqdxqtjj.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gosjbrmon.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gudzwxost.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gunqtwkli.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/geqhbqswx.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gwbixhlyk.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/geyxqpils.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gaxgpfqvo.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gatmntchu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gzbptwwea.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gvkrkwsff.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gkmhkgeqn.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/ggbxlcrrq.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gpqtgnbzj.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gyzkhwjvh.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gzyaottze.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gcinaaoog.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gdbbbqqip.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/ghfdxmopo.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gtchiquab.sHtML


<!-- 参考信息 -->