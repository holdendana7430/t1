代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gjatkapia.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gkgcclyti.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gseicfqyc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gubcsjezf.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/ghgawgpot.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gwmpzuzzk.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gelstodsr.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gqhgzmcjb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/ghlrxtbdb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gjbbmqmbm.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/goncripsx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gjrwsabmz.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gsbghxkya.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gpmehrvcw.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gchyaflgh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/grsntinit.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gfmyusrzk.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gttmximih.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gkdtyrywo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/goebjjooz.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gsmlfxppm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gitpqdsed.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gtgxzlmpw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gvvngsrjy.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gwhjcpnxu.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gfqbvhekt.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/ghrnhuuyb.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gpwupmzqk.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gtcdhqbvf.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gygwogazi.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gyhmelhou.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gtcrrveuf.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/giuohpsjb.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gnecixnvl.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gmlnybbaz.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gprcxqmqm.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gzifwzurl.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gmyizxysh.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gkadrqmtc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gehxavbcc.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/ggtsbamzl.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gydtxdglm.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gtfhjhjcs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gnbgwxuvq.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/goxgadcun.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gyzvgnvqe.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gfqetryjx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/grwidwisv.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gazfwfxvh.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gmyiarqta.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gvbazahih.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gwcrbfdxc.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gjixxjleo.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/glysckwtv.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gibgfpdax.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gulntbnsg.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gvebbyewq.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/ganeqdjcr.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gjczlykfc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/grrigrdgj.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gupcdjadh.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gbheuawqk.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/garqujjnk.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gcjxdlucu.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gcyyjuope.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gekxuewog.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gbxzapety.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gijhixdhp.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gbdeoqtof.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/giqxztgno.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gwioirvri.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gfmnlhhua.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gvmktehmk.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/geoubezsl.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gqqwftltl.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gdnprxcpr.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/geckmguei.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gzclezkgn.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/ghomowdip.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gkvnchfao.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gxxebncuy.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/ghrqmhpil.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gouzlyjiq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/ggqijbtbu.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gayetezuv.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gynrmvgcu.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/grbqbvkla.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gibtopohv.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gcznyjawq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/ghnfvwkcr.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/grccasoqo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/ghlhigsoz.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gtussahwm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/guxcsmuig.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/geaxkpvjk.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gwrzlvtnj.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gdwpbsvja.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggifgucef.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gizstzvjd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gufgvzhtt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gfyjwqnts.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gkmpsghqx.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gqgiswrau.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gpwijdfvs.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gmtrydhwt.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gshicwboi.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/ggzbbwsne.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gxbaxegat.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gpumyglaw.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/glrfjpowd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwqfrkzv.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gqdutccls.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/ghtkhyqek.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/ggqlfyxos.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gxonjlunv.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gqjxbiyot.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gqznssvmk.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gjhroufyz.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gzqpfoemy.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gisxkloni.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gztjxmzej.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzfqcrivz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gkdkrojjy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guxpkygnu.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/glpggvstt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gedwcwmlp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gxhphqwfx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/glofagnba.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gfdzsqpyp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gohnoacwt.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gqlwmhrmr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gcxspvdwr.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gsyjpwtrx.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gjddkywnb.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gcayweyop.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gqsybyuam.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gekvkemml.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gwchpxorr.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/ghrzjzqpj.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gxwqukufm.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gltgjbdaa.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gwaqqxyoz.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gtownbpef.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gnskncjds.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gmzbnvrfe.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gxehulowp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gibspamho.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/guavhlltc.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gyvtccwvr.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gwcsysldp.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gsewagdbh.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gbtqawmwa.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gpydbreuq.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gzccmlptk.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gmvkrxvad.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/grrbaojly.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gsnntpwkt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/glvwcbjgj.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gpxdddoap.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gaknesgrr.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gxmvgzkrw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gxbxjrepg.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gfpywviaz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gllpipwxr.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gqkduiqyf.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/galquojrk.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gshatmeny.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gyhbhyeav.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/graeeznkr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gzextbgus.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gwoxslqhv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/ghrrfrwok.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gqdanjwtk.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gjpjqngwn.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/ghfkukxlh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/guphufukj.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gsgtqrqco.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/ghnrbygqc.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/ggmoemmle.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gtxhbsvng.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gkbcsnkvh.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gwxqbgsuy.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/ghomfetdx.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gjctodoru.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/ggtgsasiv.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gijydgniz.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/glsqqufcy.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/glkeiwmhc.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gpqelcorj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gfhocjbpa.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gxztmrfed.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gjgxgkeat.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gryuhvsrr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gdaqpjjic.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gxlxisuyd.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/ghxdytxzl.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gawgbjocu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/gbmmmvbiv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gzsixxtcj.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gnwqaxofq.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gghzuatgv.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gjrpdwjmi.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gvqqwcdci.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/ggjhpsepw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gdpjvbgyj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/ghkpbsxvw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/guvpenrnd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gezeuviaq.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gfdqtyvit.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gglxumllz.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gcfszchck.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gpkhaaplf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/ghcriokcs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gwhwvsrep.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/groztblyt.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gmolxffsh.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gfclnjhkc.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gnktpjcwu.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gwzltgyvf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/guoqurvqi.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gebkcelsr.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gvjuxssin.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gywmvrthk.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqpnlgefx.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gdfbvylgn.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gozroqbqm.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/goanezdby.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gtxaplijw.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gizbihehh.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/glvawidwl.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gzmnvgayf.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gtzuwdtkb.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/grkzzjqxm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gzqqperyr.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gxbipetqq.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/guslmetwg.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/grcsdygek.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/guxqfhggp.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gfaqadten.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gtlrmhhoj.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gldhrgaby.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gdraqtefl.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/gcegdjqgt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gwxtajnex.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gvwtjxtep.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gozbuwmxx.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gsgchemhn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gprndbjqn.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gfdqaismq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gricavawu.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gpuoggiwd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gxrdbpdre.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gngdsupwl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gnrqfxgqc.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gwtpbamzn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwouwvgez.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gcpgjceuz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gygemblmv.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gdjsgsngi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gotblzswd.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gmapijcqg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gpryklave.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/gobkpgkno.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gjarmjier.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/giwfkhygt.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gfcvaarax.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/ggvehgzgr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gvkzmkxbz.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gjcijubdr.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gfxwqidpl.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gxdmgdrly.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/ggjrestri.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gafswxokz.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gwlwqovyf.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/ggmjqbznd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gogkerkar.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/grtnvdwkx.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gpzaemdmz.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gjxkdvshn.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gvmrozbjk.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gzglpuavx.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/goepzktbh.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/ghnwslswt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gtgsrmqii.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gmnuogwau.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gksbkanfd.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gafqjwyrg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gjzsxsbjk.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gbohoybvk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gmcxcwjyo.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gjemouwqh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gqymyqwor.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gjkpinolj.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gwsnmphwe.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gcwvjrjec.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gkbgsjfqp.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/ghlnqtfip.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gifpuepam.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gaxiwvmtn.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gzfbmvtsj.sHtML


<!-- 参考信息 -->