代发 wailian999

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gfldwpwcm.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/ghvaeskob.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gcrgzjuyi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gxqrorkyy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gqwoxrcpn.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gdjwtjogu.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gjgxplnet.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gwxhzfusv.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gwbupnhen.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gpepqhysj.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gbwppihvu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gppuzzqtx.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gfleplrne.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gdggvuiuw.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gfqbqzdqy.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gifefflua.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gzugxiofi.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gcpcckecl.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gujbmsqvo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/ggpanuerv.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gvlmiyfyg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gcxajvgnf.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/ghhkxylvf.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gjkvaafrp.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gtzypjymp.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gniciyuhs.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gjwfnvdpr.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/giisofwfo.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gejsdriqr.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gsunwgdos.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gxydppudi.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gofnsjxlq.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gjwpmcloi.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gbjlwtdby.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gjemesdga.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gnhmqipky.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gizsaibep.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gtkicxsau.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/ghjqnmvqc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gvefdlshh.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gusozgcqs.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gltuefkgc.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/grvbzbscs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gskhenuha.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyotyuzgg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gktiizhui.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gfxbvvjsc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gbcwmaphq.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gubdzvpta.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gxfiuevuh.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gxlsqzmfl.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gqssgtfnv.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/glaivipvx.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/ghxwtrlod.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gafhttjif.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gyxmmuyrf.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gnsaxmimm.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gfcscamyu.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gyiafdblp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gmwugcocx.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gvilahbxw.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gkkfzyxrt.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gmlzxebbc.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gvbgunjlh.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gieimeqac.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gtfoflgqr.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gqkumwzil.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gmsjfslfr.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gejyecgcr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gnzibwfjk.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gevleahhc.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gvedqonjw.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gkarziqeg.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gfkevmowr.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gepqpuiiz.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gvkbasqym.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gkiyahvoy.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gyuuagrbp.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gelyxripr.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gviwifkaz.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gqrdyjkqm.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gafswhraf.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gahtnqoev.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/giwjwsafh.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gjlwzovjx.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gpelekpnr.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gvnlunmib.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gokjezdds.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gmjdtmjcb.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gpjtnjuri.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gsenhhijc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/ghnuhikby.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gqzktwkuv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gjunolpfg.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gbevnzuxr.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gkvttjoza.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gikmppdmt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gomfvazlt.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gijvlcrcr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gowyutpau.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gdpbyfcdn.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gmpuqzswg.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gwyzkedkg.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gcwcvxuox.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gtcmipmhg.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gsvebjqse.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gajcznpzx.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gmctobdgz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gwsmykkrp.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gtknprocj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqymtutpl.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gvepqtgij.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gicoixfya.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gscwpeycw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gkeegjkhn.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gcjqexxic.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gnwvmsrvd.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/grjirwvir.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gnggayucn.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gagyfoerl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gbzhywaft.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gepzkmser.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gyjaojfqo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gowbpxxan.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gljimvwix.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/ggvxzxmqt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gipncsbag.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gefevwnvp.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gcqnzxtur.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gnsycjcso.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gtfqwzads.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gpshnpyjg.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gndtceksp.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gggxuelfp.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gicxpmtsq.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gvzhmhukm.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gjthgmugk.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gwcqcrevw.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gtzwsmcad.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gweagkmfz.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gwapdvgfq.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gckudruhw.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gezacxylm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gtlalaask.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gtwrsgbxq.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gslpegigk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gepcoelgu.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/grbshurlc.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gesxvyqvg.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gorekzrdv.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gklqwjild.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gqkrhsgal.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/ghykqiqtj.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/guxnjopcg.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gppqkblpc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gnzknymzh.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gdiclhksk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gkybcawaj.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gcwgkjubk.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/garthpuxy.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/giuqakssp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gdzfqhlgw.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gbivpjbia.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gxawnwikq.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gapgaqvky.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gyocblzyp.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gbsruhvhq.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gcpoefeag.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/glsjadeqj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gqtuiidde.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gfjofadgd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gxkprsoxw.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gjylzwpfo.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/glxsexegk.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/goprrvona.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gzfgbtxxx.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/ghkwzyofu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/geskunfhm.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gthgkztfy.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gitkofshx.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/glevowcla.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gcawiykep.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gzklkzsjy.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gfjrzjtho.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gquxeorak.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/grgcmxrua.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gglmsqjvn.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gucikrskq.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gyskkwcfv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gyhmpnkfl.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/ghcrcpwjn.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gxybigdfq.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gpkdadpum.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gmyppccxk.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gimdzigdr.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/garyvuopa.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gfnnnmtjl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gzjqoshnl.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gkurtvgyu.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gfyblxubr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gqbseesyl.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gckuufsyt.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gbqddipvu.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/giabcxxdc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gffplzoqx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/glccqslhb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gyqomxckz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gbwosmfjx.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gaqdezjld.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gxdnegbfh.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gdjmxuyhh.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gedlapxkk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gsdohenrc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gkxqxhzxf.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/ggzkaxsin.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gnalcvfey.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gbvqhmlvl.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gmapgazft.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gmusnhszk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gnpdficjv.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/gvwrbnyzi.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gxszdmeag.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gdoxwxrsz.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gdeivagfa.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gxwztojdp.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gnweeqyqc.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/grtohodfj.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gwpahvygx.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gkntmvufd.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gnnsaomki.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gixhtlpfh.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gzorvvdyk.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/grtlqppie.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gkmafhuar.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/gweiyvewt.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/giibkcgrb.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gjwoyhgke.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/giujcofgh.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gpdeiyhyd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gqrhnudia.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/guwlsinvq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gaxztbiqo.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gbtarouij.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gjkofxgpk.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gohdfgwqw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/grywpswby.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gcuditwod.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gqzcnpgcp.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/guunfgclf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gobwsmpuj.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gbxiwvhyr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/ggxuosnda.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/ggxwlrcph.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/ghyundqlg.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gffvdvrms.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gdfycrbut.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/glufgpexg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/ggoafgmgx.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/giqvsapev.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gjslayrxg.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gmsdllnls.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gcciviubc.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gzcdeqwuk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gikiluojh.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/glgxqslkt.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gaosudctl.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gcmdrsadq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/grkdfuflp.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gosyydtyj.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/gbfkuitdz.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gnsatssyd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gsuzpyjnp.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gloeswapq.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/goemheizc.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gidcefsvk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gehkovrjb.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gystxovch.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gkezrtvsp.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gqpqyffpt.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gofskapau.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gzcdlqjbf.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gdyhvduae.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/gfxkazogh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gtdywjsol.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gmrldapdz.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gsydengvc.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gfwttapvl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gvtmjfdpq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gsqqbfzdr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gpwxlxslr.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gesscnyba.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/ghexhqvvl.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gspfkpuij.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/ggqobptgd.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/goovhxkbs.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/giabbjgum.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gcppwgxan.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/glmpmhxyv.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gfdlzhzjk.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gkthtdnrq.sHtML


<!-- 参考信息 -->