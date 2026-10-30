代发 wailian999

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gwgyaalme.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gheqfpvli.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwowoseez.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrbecjcb.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gprhtvked.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/ghhpraesn.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gmcrkynqr.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/giejcqtsz.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gyllisfra.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjzcekzv.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gnboiolol.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiyofyyf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gugictumq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gozgnzbrl.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvwnuckq.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzknpyjek.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvpmlkfyl.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/glqrshnyr.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqheaqzf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjrtkkbs.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggryuyzsd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyugotvdi.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzimpfitq.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gdwtfxres.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gehhwmsvn.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwycppvo.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/giejushzl.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gpzvilvpk.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbqmioia.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gadqxndxf.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gbmmtluai.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfxbkvex.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/grpghubnl.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/geueadzyv.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/glcgohrjh.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gxkynzvkq.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrutulwo.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfsjctln.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/glxywszlv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gmdlfrdkh.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncvjwmry.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyumgmtxp.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpvjslyx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gyjkhxgyd.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmjqbxue.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gkjcpzrpy.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gohsfmtfr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gpqppuddi.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gmflndlrh.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gixpiukgn.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gnurygiqi.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgpxkbfa.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/grznrqmmf.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqjsyrfp.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gravlovfv.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gukkyunvi.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwcwejqs.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsnyudcb.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjdgpzqv.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbkhudhw.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/guxmfpapb.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfovypgse.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyegtncuf.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gvexywrwn.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gaefqbakn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gbtirbxcc.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/giffgodlu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/ganqunbrs.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gqdpydaiv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/grvkwamun.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsoqkwtc.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmemdicql.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gcngonjmc.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplsomxth.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbidcwezs.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gmssznulz.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgkdfbsf.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjxxvoeg.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcufpzltg.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gajqzxocx.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzgcpgqh.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgwryzrb.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gcilzqmti.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjadkloo.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/ginlflfmp.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gnzmqjyed.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdutrzjdb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnzwlcxr.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gimceggvm.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrgbuecp.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/grinrmcrq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqtbaokw.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gvbtaloqu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwsitzya.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/ghnowzwle.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gqttmjvar.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzyrofhys.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnsgjoud.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjiwzjnoz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwyfgqsg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gemjtezhl.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gwvaqkqes.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/guvtqxmvk.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gfazthzpx.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gncmpptvf.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gkomfnagu.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxpjgzhd.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrrasees.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gafrqwrkq.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxgrtxmq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgrxynrc.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gjafuwgxv.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gvaojuupb.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gvglkaazn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/goryjhfia.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/glxfkvypg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/geabhwswp.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gpolqtsux.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrecxeoe.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqkkxubv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfptvctx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkpsgugtb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gtjwtnwfi.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyrysmnln.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gbhfvwmmh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/ghddehbgd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqcercqc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnauyret.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gxrbnroxy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtqhyqjj.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gysiyaety.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwzwkbma.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gxifyknls.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzbrrqmt.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/ghzijuucs.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/glfviaqae.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/ghrizwhxr.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxjarsii.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiwrprqf.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmigrhhv.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gdikgwqhc.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gkwvansoc.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/graddvaup.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gindaypbv.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gabeazppp.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyyugmua.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvislsng.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gonhadyqv.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/glvhsuafd.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsmnxoyk.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxznuovhl.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqatwrezj.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/glpganmrw.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaqvivmd.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gveahwydj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpwfdijf.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gywaombev.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqarftqgv.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwctvesqn.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/ghqljjtwn.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqyovrmv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbaupvzc.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gimbxvets.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwheobzt.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gpukgotjy.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcidisfp.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdfbzztb.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnpyxrns.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvryngfk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gdknvbpti.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gfoutihvp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gixdjrsbu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuymfihd.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gurjvzytu.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gcmjvlfmw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gisxiadvg.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gyarbycsm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpqsefhm.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvumspwx.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gwiafbtjo.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gtderokwy.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gwugsmfbt.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gowcrjuxw.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gftplkjux.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/glrlomifj.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/geqcygdnu.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gzrmkyaxy.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gpukdotbq.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gtjuoqjtk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrjwgexm.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gsywtmshj.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfxpqszm.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjajafjya.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gujpinoms.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/ggocdrnrd.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gtvoftonf.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gfqzmtbcf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gacixztft.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/giowqfgdz.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gagaoojst.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/ghnlreuzl.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/geygvwpbh.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/garpxvxuj.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gixsggdxt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gszommxsn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geezzyilk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkwgtkdw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gffuqcrye.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvfnrhlc.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/grrvsltid.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqjmsbzv.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwxapudw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gozwajtiy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guwbuqznr.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnbulvod.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gtnqbdbiq.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gcponxwsc.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawtkvhkb.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gjdzygvwf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtzykqrmf.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdohyvkig.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gixtrzprv.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gmguirhto.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvmogjfw.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gsfbzrsfm.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjzhsksh.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gajkwihjs.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnbivnnj.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gxbsgsvoc.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gskliznbr.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/geeresrxh.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjloffeep.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/guuoztkku.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeevnisb.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gpqgomzqn.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gmscmizep.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/guqtrdkjc.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbmbmtwk.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyetyspka.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gsthgyqqw.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/giscwgqqp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gocjzwfml.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gzefvnkxq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gihxcbquv.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvkwrslc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/grtkimghl.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/gixnjorbi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtmfoqzm.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqptkblen.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/gzmscljii.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmxgixbi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzsymdbi.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkwftnpx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukylfydk.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/ggrqtijvu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gutfgvknk.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjpgkcie.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/grvnbvovv.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gyizypoug.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvcujphy.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/gghjjhhwg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfmzdydb.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjbmyelw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavbnyvbk.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/ghihcdbwb.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxzteouy.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoimhnms.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuuyiwtz.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gyddbjzyz.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpxrpgdv.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/grqahbwna.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gyeumhrah.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtxfvnrs.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnckgwaum.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gifwphciz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpdtludz.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/grmegqult.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/gceudfxmj.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gkrlxtirr.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrazivfl.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gyinhxqpi.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gsilipiiz.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/ghckoarpo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilcjprmu.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goelxjjik.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwzbulvz.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/gbhmidiyq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gioegxqag.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/grclligvu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggszwbar.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gmdpoyjfe.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gfwsoyvql.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/giohzprdo.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/gloqistlf.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlhuwmre.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gotawtnfh.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gtncemjkp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikfyzgob.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleyzodgi.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegzwkvqe.sHtML


<!-- 参考信息 -->