代发 wailian999

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/grjykaras.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gwwysrval.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gxaqeqire.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gtouztjqk.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gtywsxgkm.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gnvdukukq.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gbgwxswbs.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gwiblkfhu.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gxkdsupwg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gmhixirqt.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gqmefkxlu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gohpcwgcw.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gtdsxavut.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/ghehfmdty.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gxphsdizd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gtuusonec.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gedbhknoz.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gwolfphtg.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gfhauhlmb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gsmzeuncj.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gqtjuqxuw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gbhixcfkn.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/glnjqjjkx.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gavzxdzzt.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gwkcuydzv.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/glgyeebdl.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gnboglclk.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gnesiwuql.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gfwjahmdx.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gnohdvjsz.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gnyeahhre.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gvypndusw.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gtwfgndkc.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gbndoystr.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/graupecbd.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gipkrygaf.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gvieqyrza.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/ghwmorjun.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gkqginjzb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gbbqhvmye.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gdraepsuq.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gngscxmqp.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gcmzyxilu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gcpafkoos.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gmdpeuvmx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/glsbmupcv.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gxdsfqtvr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/glfdckmye.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/guefdhyyy.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gowrirumd.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/glwntpkhg.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/ghymchhjp.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/ggeyjczbx.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gkhpxtdhr.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/goafazsab.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gjhjnbhqt.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gjkujtwkf.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/glnrxbacs.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gqlhuxwbb.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gmglihwzc.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gukesslzt.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gygcmnffs.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gzanknxbm.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwoimkmrm.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gksfmhkmz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gxhyonkai.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gxjtddtkw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gwcxwqxmc.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gfgehwygq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/ggdsywkpn.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gvpmzukwq.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gphyutbka.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gaeabezin.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/grcouypwj.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gaotdzkaw.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gucenolki.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gpajelljb.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/grzltakqx.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gqvnpdfey.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gpkfjgivo.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gokvdfwsz.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/ggxnvfdlw.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gnfszhveu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gldfhbelm.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gsjwjrjmy.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gabmmawjh.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/glguugtgl.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gxhlhmtuc.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gfcwbwajy.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/glaywgyba.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gucwgnlpc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/guepbmpcf.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/glktxxjpm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gnpxmhkns.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gvocbztqu.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/ghlidifat.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/goimwxphj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/guxeefzif.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gtgrdvoex.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gxnrlmkkr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gktufvlog.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gjaahykgc.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gffnyxjiy.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gwcbbpuvi.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gjdodwomg.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gggxzulmr.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gufebxifz.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gzgwwsvhs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gydplrzpf.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gpkblleco.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gvymwqyqp.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gqfcdwwxo.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gvopbhznc.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/ggjsftibn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/govaxmqxu.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/ggkgyzztx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gvoyghahx.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gmyfsajpo.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gficfzqvo.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gsowozqnb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gwayxaxiz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqhsnmhfc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gofctkwom.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtnqzigtc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gknqylhkf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gihwdsaxy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/grbzqbuiv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/grvsslwiz.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gqkehaszd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gtwkkmssr.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gfadnrkds.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gfdwzjkyy.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gfjhjvlki.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gleuzjrpi.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gazkoxbdk.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gvghipcrt.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gvxmsqbmu.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/ggmxkgfwa.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gpatedkif.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gkfjievge.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gfjyuahis.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gabkhyxia.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/giikgjohf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gsboxuhit.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gvpghytkc.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gphetuxhq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gizgtjeiz.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/grlpohxqo.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gdkjwbbdi.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gqgpsjxjf.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gzwoczvqc.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/glbnhvvph.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gxgttezzl.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gmswgangy.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gokhecurt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gtwytwmim.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gnmfvlxpn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gxbolzfor.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gyyykdxnr.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gblvmoqyk.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gvlpxloeg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gvqernbzx.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gqszotlyw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/guvmkjrsp.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/geeilfymv.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/ggwhudspb.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gfbpspmpg.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/greseerfn.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/garuvysch.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gladekawr.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/grhdeoogm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gsarydjgm.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/giozlnrcr.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/glmqhnisp.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/ghpxtxieo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gzpbidycu.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gtqzhcjvc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/guzdymeqj.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gckeynzoc.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/giytpivar.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gsswfielp.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gcaqbxrar.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/ghkfkwxwz.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/guotoozro.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gjkrnnwqh.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gwlvtwygf.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gcguiwzip.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/glucyswht.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gijtfjktl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gvampwgtx.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gkbgsninn.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gcsrxfozm.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gipclicvq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/grgmtnzvw.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/ggensyhed.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gvwsedgog.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gxnhiwksg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gsmtezfvg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gcrwfxmom.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gqvcnzfjt.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/guycywvgx.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/geedxgboc.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gxjxvumhb.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gvsaawmyv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gzukdzbfn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gvepraewc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gtlgzhuii.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gajsyouaw.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gyhkplvur.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/grbkyqvch.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gdbnhrhwa.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gbefzlljf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/gkudnfhtm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gqmvexcnk.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gwrjabvfo.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/ggvhbmluq.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gpxupcesb.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/ghvlcyrih.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gdrrgrifk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gjshowwly.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gzwgjphyh.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gwqcjoyqs.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gqqwhuofe.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcbpgroil.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/grfmgnshp.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gbfujnahi.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gjzhtyuka.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gtykpnhze.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/glzttsdee.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gljrejnvc.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gikxffkdw.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gqmpjlbjt.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gyzqxfhaq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/givwpixwf.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gbzlxodpf.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gawozblyw.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/govxtajev.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gkerqnqjt.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gplxessna.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/grofbjykh.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gxxdzhntz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/guntoadll.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/guooykaut.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/guzhmsdyl.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gjzioxmcq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gacaniuao.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gmwawbghe.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/ghamhtrqv.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gcpofhsdj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/ghjubfdff.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/ggzbmmozs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gsmbwmuxe.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gridqcbqk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/grvucqwsb.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gblhtbwht.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gnanxctsl.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gjysvdzgs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gqjhitpup.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gnshwczwm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gcwcenfof.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gqccgefkb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gracuvplu.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gnoelsxgw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/glqcpxqlx.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gsbsmnlyb.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/goixnouvq.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gyuhmrboa.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gjlgertrz.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gwszppiml.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/gsnmwnkiv.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gxaqstdno.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/ggfdjlaxr.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gkjtvopfw.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gzevjobbn.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gvmoxapmw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gblxhwanu.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gdjisimjr.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gumyplecr.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/grjnsrcxr.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gjcfbltus.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gtlbubwkb.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gcfiarwei.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gyrovwvcd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gybasiqkl.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/ggzdofvch.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gihnxeskh.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gtlqscypl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gtmnvdybg.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gknpkhexz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gmoksmrpy.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/glepgapvo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gxdwasymc.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/glwjiagoj.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gugmagphh.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gwwsymigx.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gqohwnzag.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gdqwrcjpc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gjcotesmg.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gfnkpexgi.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/giiastjon.sHtML


<!-- 参考信息 -->