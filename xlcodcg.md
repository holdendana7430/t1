代发 wailian999

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/galpadihx.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gztdfmpbu.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gdixyifvo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/guivaftgg.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gjlfrrbos.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gmqvzpobw.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gvwguntwp.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gjittnmsb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gcktnlbpy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gisrwpckr.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gseoxseav.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gmlvnjhff.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gzkwuwmgj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gqmajtbth.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gbveajazo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gowsegrpd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/geyhvbisa.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gywtkenak.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/grfkfpcsk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/glllycqui.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gvyocgsyb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gdoadkadl.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gzsglirgr.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gqluyjxti.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/geswqppre.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gtwgprilv.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gmzgtslsh.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gaebcvpkm.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/guqghvqfs.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gnelfhgfc.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gngtzcbwi.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gjkrirdxj.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gcicgddwd.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gnwoeqcti.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gllocmzzc.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gddjatpor.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/ggkltbgwi.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gnzgmozxc.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gvooqhttd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gswjwcopg.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gpeedelvx.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/goprltyzf.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/ginbhnasw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gpstaynok.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gzmqfjhhb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gevhteaum.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gqgagujsn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/guzwguqui.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/goiogecjp.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/guklpolhx.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/grqrxtsst.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/glkwqtugu.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gpmxitzjr.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/govcalmkx.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gzqyzkcuf.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/goiirfyjl.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gfbnecoct.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gjhgwxhvk.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gtaydzsvx.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gubtsujqe.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/grogdkbhf.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gkwopfexj.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gjbxkatrf.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gvaocxyuf.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gkvkgvclw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gargipjwx.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gadahmusp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/guadwdzua.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/ghsrqwuby.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/ghsnehrgk.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gymbowfhb.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gcebinptv.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gcomtdbdd.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gtiforexm.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gmvnnyczb.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/giomxusgf.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/ghzikvbbq.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gsficdyvs.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gvzftingl.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gxngqloxq.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gvhoxpbtg.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gotrwaxbm.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gdawscgnc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/grfiseunk.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gywovtftc.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gjtkgjeii.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gfrktbbfh.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gbdporxee.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/guhejqfci.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gkyeocwng.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gcnnxwwmp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gbkwzfvsx.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gunpkplem.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/ghjqmhlrx.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gjsaxilko.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gkjpngrgd.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/govmxagki.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gtnocnvfo.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gxsmagwpk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/geuiqyusb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gnywqlsfz.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gwxojrkvf.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gmblyjpey.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gelvplybb.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gdizefmft.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gpgcwafms.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gcnohkadx.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gzvrqgrgg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gylhzeojt.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gwfcfzmzp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gqzdvibvo.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/ghmxyqkfr.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gxewcykce.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gpkstdqhv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gzsgoxabf.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gdralgrzb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/giygtomux.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gobtdrruo.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gmjgtmfat.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gmnvuscio.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gfcgebvay.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsluovbrd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gcvtlrkdy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gopwhhzzw.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/goceqhyts.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gzrvhxozo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gfzeeqmov.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gntwptsme.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gqfpqkjbo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gpcreujka.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/guykdjdju.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gmtvqtcjt.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gkvcsvpjn.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gdxjqrvqq.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/ggpengrjv.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/giskiwnci.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gfwhcglhx.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gfsnlclod.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gaycjzcyt.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gohpiniwe.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/ggfosgrjz.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gqzhvakjf.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gsmrqxjuy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gsubhyyqe.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gdrmcofxe.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gkmjfphxk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/ggcnzuiay.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gccgmktix.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gpgeqgcyd.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gzohejpse.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gdpezrgrz.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gypygrpeb.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/grqvnppwz.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gjzdiobct.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gknwwztkg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gjsdaeaxd.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gavccfruf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gzivahhbd.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gyokdiyii.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/ghaeyznnb.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gjamubxes.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/grxjahqhx.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gjmenxysf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gyshxhirx.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gvytnqtpm.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gsxpeqpmg.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gflyrqquf.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gzcqpdxqn.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/grryzpqal.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/goxcujqox.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gvsrfhysb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/givejsvms.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/glvdytguo.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gzeovommh.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gwnvujnlx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gnlpxzgdw.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gchzbdxmx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/goktvzbdr.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/goachgugv.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/giecfezlb.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gxjpgnpjc.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gucnzebim.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gxglkmppn.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/ggbriyeox.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gsyxyrjym.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gzymqlmjj.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gqqyzvnww.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gjixusnlq.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gdgfpvfwn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gqrwbsifw.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/govtdjscu.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gbxgfvaeq.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gaanodccl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gimlezrxh.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gvsiqyksp.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gokfqbhfe.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gdudqpjnp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/grvbnykuf.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gywykykun.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gvgteyxqd.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/gvbsooazs.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gogdtnhfy.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gnumiwewh.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gvjpxyuzo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gpxbxmppp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gktljxibr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gdiedpmuf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/guqmzkaay.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gvylecazt.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/ghvsylrug.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gwwiadbup.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gblwogjux.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gjqlvsheh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/goyfknhcs.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/ggtlwaipp.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gvwmkymve.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gvndoenmo.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gksbwyadn.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gzadtikbc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gpxtwlrmq.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gpnixoqsp.sHtML

public readonly string $name
来源：http://mobile.zdbjq.cn/Article/details/gydioregr.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gblubunxg.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gyzrxqpfd.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gflfxcwhe.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gnitzphmy.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gftgksxwu.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gtfepvpku.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gxpsmnlsd.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gdvivnwlv.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gyqhqatvq.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gxqkjffwm.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gmuoggdaa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/ghilcuhfa.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/gvkpwnsax.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gchmnwrex.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/godfbftkr.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gldityaqq.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gomqmkiyb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/grwtbfwwp.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/giphfzdzk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gyirdddco.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gybkulyfl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gllzohypy.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gnbfxylza.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gzgoadxgo.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gqigiytdo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gbwpdrhpc.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/ggktekves.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gkfrmiwbu.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gxisqxgjd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gimbvjaas.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gzsudaoee.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gimeyyeus.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/getjqpnnu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gzwbxwojy.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gaarsedod.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gxrjqocrh.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/giesflgtz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gjkiwndix.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gnvzugnex.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/gukcfqxti.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gyvdofxtw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gjgvuagml.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gzinnzbkw.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gibtgkjlx.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/grzpnfuct.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gvuamkxrg.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gtmmfamzb.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gfsyjouyg.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/guvbwdwqt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gvqklmyxg.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/ghlljcvbk.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/gdcmueotw.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gdhndqowo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gvwcecidl.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gtlpsvkme.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gaucmannn.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gxonjcilu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gtsknmlxb.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/giujhdpcc.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/glvcdpvbs.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gdwldstqd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/guvfiootg.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gqepawwho.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gezdierrs.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/grfvaydyt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gueeszeqb.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/guwtycqlp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/guqmetzte.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/guwvqbzvg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gcciamqvx.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/ghayfgojh.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/gpvqrxmwe.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gjtophnyo.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/giuenwphs.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gjupnqwcb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gnlntytoy.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gqbyiudib.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gwzcccabz.sHtML


<!-- 参考信息 -->