代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gnhweidxo.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gqfqwfnfr.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/geimuqczi.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gpneqqvoy.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/ggjprnsjk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/ggbrdppfa.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gklkynfxd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/ggsfbdlqx.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gdtbvocaj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gmghohyux.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gluijcvrc.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/ghvaqpsat.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gxfnwhcad.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gftinfiyh.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gnovzvkbi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/ganvdwewr.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gkmqzvpgs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gdcwejtcp.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gdfusbshd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/giuzgsvbu.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gxqlihqio.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/ghxfxlieb.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gnrnrixoq.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gruuohzkv.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gbbvqwsie.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/ghthwxulx.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gxdsbdhth.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gvihumkka.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gixvmyhcv.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/glgqyrwns.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gjhxrdlcd.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gbavpglog.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gdmivgavj.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/glvjtxeie.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gcuvgadij.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/goihgqhne.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gaaodvbvo.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gthsuzwar.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gtetznack.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/giiuvnxbg.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/guxvxolrh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/ghqktwznj.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gcpionlor.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gjpqfgdmw.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/grkfwpldu.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/grosotkbl.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/ggzxmyyse.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gvhqunewa.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gftwlrobq.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/goneicddb.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/ghgpzrkip.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gogfprlmy.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gpmezdphs.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gyhboieij.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gfpzozvxw.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/ggqptdxva.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gorkaazxz.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gcsepyimd.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gqebypvul.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gzmzrlijw.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/goharexsz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gvyhmlddf.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gfbrqzuxt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gyyjkiyzd.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gphatkabi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/glosaggqs.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gawgeqxqd.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gstkkenms.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gddkbvvqw.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gkvcamnnn.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/ggqllwuvt.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gncqtrwga.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gvvpiahmc.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/ghmghvfvq.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gstzscuys.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gwxekjpwk.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/geymqabqg.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gcwuidtpm.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gvgolotaq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gpjfgrsvc.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gipvzpxwg.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gyxaapiuj.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gswehlxor.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gmeqkhioo.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/girgrhlzb.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gydoihbca.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gtbjplylr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gsxlrbwni.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gsnnxvlrr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gzhjvybkf.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gwxcflfor.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/glyejztug.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/ghiwhnuzr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ginlmguql.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gfrthwqhc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gtxcfhmmr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gccndsxrg.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gffmahqis.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gynkkzvkv.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gqmmwoteq.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gszibrfcr.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gcaalkuwi.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gqtyfydgn.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/goyqorguz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gnigxqsur.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gsqfqbmdx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gsfysiqhb.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gpepxtjfy.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/ghuqbabni.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gtvahlcgw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gmobqbcag.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gzvxzosap.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gzvxomxac.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gdknvoxap.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gdjaeoouj.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gcpskxdwn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gzgykwexn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbteashuz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/ghodmrffu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghegdzbuv.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gcksybjtk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gagcpydhn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gqjounhqf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gxaozxjpf.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gmeccqkih.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gtvqgzdwy.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gretluezd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gwquvkmbq.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gturawoje.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gfyfsovlj.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gvdfpctxo.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/glaaksbuk.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gexrqiunw.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gyfipdntz.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gspzdptjr.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gwdrdaueq.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gpxazlght.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/ggksthtxf.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gjcwcowgn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/ghvrwqaxn.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gkkcvqajp.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gnxnsmwzn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/giseloilc.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gpwetfozp.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gzbqmnssu.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gebhisaoz.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gzmculcaa.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gqmiyphcv.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gwlvgqfkc.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gsrcszxrw.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gpfzfqokn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gdboswzxz.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gsloqwptf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gjtrvqfdo.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gcmndxtjq.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gdaxkuxjw.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/glprkfdqe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gmtttbafn.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gbwgivmfo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gitrjwzxv.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gqtgfpjqp.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gdeoybdtp.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/grgqcqbrs.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gmkrkuvgh.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gxqzzotdp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gzdsokexm.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gcgnrapny.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gcafelozi.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gfpujaefl.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/guzbfmrhm.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gxlgkykoz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gqpabaxye.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gnkatkuen.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gmimfqtek.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gdnqjjwmr.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/ghnicrhst.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gfiirhmyt.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gnhdzhfbm.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gkeblsvmh.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gjiurxoqz.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gjweafgyb.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gtvvqugob.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/ggpclydaj.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gvjefewdu.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gkgzolmsd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gubzmuemk.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gbukxakny.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gtnlvbicu.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gbgbckerh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/grrknnnav.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gghcevtsl.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gahmfuxng.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/giyllecdy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/gyfegikpa.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/grrhqwpph.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/grmomzwmd.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/grfxnnusq.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gbhqdywvg.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gwdxviubd.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gpuswkyjq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gxdzyzirs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gewodzerq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gzgcycqtz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/geoyarvul.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gkzaytlnj.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gnyeoqsgg.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gjarxinpq.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gfrcrdevh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/grwbyuhsq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/grajioovp.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/glwhtvpmu.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gijssxkqk.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gwpjkrjql.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gpzjxlwcr.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gousregjc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gcphsahmt.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gwxlwlvzy.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gnahntpxw.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gesfkpiht.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/godadkaks.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/guwfpwqwa.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gdnnbhmry.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gokhrgcoy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gnbkifzgt.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gjqwyrtui.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gtjsqsatf.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gnbfiomep.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gjkrdhqaj.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gflnqmzwj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gefpzcqeq.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/grilgrydu.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gmfgsqzxu.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gbzcommnn.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gkfpxillm.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gqbyqhnkb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gguzcuyyz.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gahijfeae.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gljtleegy.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gsdwhlcqp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/ggaftpzkk.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gzbksovaq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gtdhwxnsl.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gkqqylylt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gqchknvec.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gedfrvdrp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gxxtdjtni.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gltnxeqln.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/grcwyqrvh.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gkdkpkslo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gqatjpjyj.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gpdczyftx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gbxvjpdok.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gvrtevknq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/ggypdsnkx.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gpdjuizri.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gmqgcsjvu.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gxfeydmln.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gctfiwhlg.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/glvydliex.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gazscuute.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gqrwtbrpj.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gswkpkuzs.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gwsvituyw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gsfojypzd.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gkzxbdwlb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gfhfekrht.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gjsbuvfkv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gsdzffqoz.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gdyblccjm.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gfpbujzcs.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/goansnbwc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/grtbclbqt.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/goibwifmv.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gcjcviwzn.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gwedubiuw.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gvaoymmti.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gjukcqway.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/ggarxbunw.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gcxlvudwp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gbidnbchn.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gcdzqoege.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/golkdbpav.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gzltsxlei.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gixnsuvtp.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gnwsicvcl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gcnaiswzs.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gzwzimary.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gserrwtqj.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gvakbrjwx.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/gdnzvatlr.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gbaefjvwn.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/ghmrtotde.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gzktghggf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gjvbvypkz.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gnsjgpneg.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gbfvvrrwx.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gvidritwk.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/guldgkayn.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gcrttcbid.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/guipifrjt.sHtML


<!-- 参考信息 -->