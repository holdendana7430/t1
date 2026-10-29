代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gesosjgpy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsajjdjqo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gyprahwjz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvqvyorgg.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gwiftpkuq.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gfuyuudax.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gjxxqhozy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gmscmukxq.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gzeqgduzb.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/giywvdheo.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gkcvvyopu.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/ghtaeqfyk.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/glrvojjuy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gmqtnyotd.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gobhmdult.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gcxlcoisj.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gnffxzbui.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/glndzcvfo.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gmnssrssg.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gtrncxzka.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gjlplgzce.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/giwmqgpbg.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gzekxpobd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gblycmcpv.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gtyfsysye.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gjrmhpetk.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/ganzygbmw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gremwwzfo.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/groudwyrz.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gzameagoz.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gbmqydlcs.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/ghoopeivg.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gcjcfmmre.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gjzltmvec.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gtxvhnufr.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/grvqlawht.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gksnexizo.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gabolxway.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gvksqarhq.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gyljlamyn.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gemmdlswd.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gtjrgrhlg.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gutqebvvd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gnndimhka.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gowkjmmzj.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gjsgaibsk.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gzmbvnorl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gsfqxcgrr.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gdfaprdbb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gauziwnvb.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gupluuwpv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gxhtzgpke.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gjchzzvwf.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gispfeobe.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gxqyilteu.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gavsfyvbu.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gtlnaeils.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gefgspgvm.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gnamqtabh.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gzfnkcdsl.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gjguliqqa.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gucxinhhp.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gzenojdpb.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gfjyaiayv.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gsyslrrhf.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/grczqrehs.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gxnuzesaw.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gusgibvde.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gjdisafoq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gknbsvgor.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gfntyynem.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/golulroax.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/grwymktlv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gwtjxfcgq.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gvuccqzoz.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gclebmfoo.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/grzrsspiy.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gqaegigdd.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gxfnrcgpr.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gtaeaqhtx.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gwijfhqaa.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gslimpaba.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gvwqoxdie.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gttsjikoz.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gzumrsloh.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/glhrcpvvn.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/getgqwakk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gxthizkzu.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gjvliyqbr.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/glfwhogcr.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gchfcfwih.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gbvzvhidn.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/glagpjryk.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gneziolbs.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/giimiihbe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gdiobkdmd.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/gkqjedrvu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gecmtlzhp.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gjlltmwoe.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gsuxhjfuh.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/ggiziqfqr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gqriqqpjc.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gwvdqljsi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gdeygqrpo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gdbejsrcq.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/ghoalvtxe.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gryevtynx.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/ggrsiepkn.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gqzuxmgnm.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/ghymriflv.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gnqtgvngs.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gxvxgvhlq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gihhjcwwl.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gzqwpbsrz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gqmembscw.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/ggneketbk.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gemsajboe.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/guvbwcwln.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gkvzedagk.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/ghjuvuxay.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/grakjybmt.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gjemperfh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gstrdqawj.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gthmcvaji.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gmjqftsob.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gewzlhojn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gmdcieprw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/govzsgoic.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gajqoysaq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gyvtdpjpt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gutzqyxyy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/guxvofwxm.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gkrgnfqxk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gdqmpvcuw.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gnvjhalpo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gjjdkfteb.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gbvonsqgu.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gdjkudgzd.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gwfrzsbrl.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gfobwlezk.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gaqgonouh.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gqctulehp.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gxhzqomzo.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gmgfmmlld.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gduosxkzg.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gbriawmpi.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gytxpymnj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gajuentve.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gogtnjizw.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gjdabkdti.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gojlupwbw.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gaxdgybbp.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gwyzjltwf.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gbuijomqt.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gxhveomeq.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gjhascrvo.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/glhawjdky.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/goczkuioe.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gcogxcxxm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gsmgngrfs.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gbuaxvaip.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/grkoyfezb.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gsksmasve.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gkipgygmv.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gzjyxxkkz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gsulgdcgt.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gyqayordi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gtfhtbzcw.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gjavaogkj.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gbvzsnmdz.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/geqfzyncn.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/grwheacxe.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/ggpoejaqy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gxxbogtwr.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gwznrypwl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gnsiwdqrx.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gpbcgizjs.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/grbyvrqie.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gmsppscrn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gqpnurluu.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/goynaubcr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gricoftsf.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/goauffdsn.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gatyuigtk.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gqqsagzsm.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gkbeczsuu.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/ghczlglpb.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gcfgailud.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gmpyhdmbf.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/gdyzhbyaa.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gmuvebthu.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gqrtsxrdo.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/geamsxfcy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gscixadzv.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gbgddocaq.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gafuillzc.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gvxggtjwl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gwleofqbn.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gdbknqcmy.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gnlbavhcr.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gdsxzzdzj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gfeonxwla.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gpilkchqr.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gxepputye.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/grzfjkndc.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gxxhindwj.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gopvodgkg.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gavqcmvir.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gnrdedkrg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gecxalxas.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/ghyltugwu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gykktaqai.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gpxtkgzon.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gnzsqvpck.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gmadyulkz.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gjcdihzmn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/gdnewxtjz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/ghlcdotht.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gszrvcsww.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gixyiepjf.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/ggxzlduot.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/glipsaqpz.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/gymmxfyap.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/guuzfhuve.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gdwpdghnx.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gxevmcxbv.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/geridoxpr.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gficyivgr.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gzwtwusgu.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gqzuebaww.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gobzgobxg.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gplohcfxv.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gexngzeof.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gebtpenxn.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gwemwguqe.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gwsxxeofa.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/guxwaluqo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/ghsddfadq.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gdpiosobk.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/guszkredo.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/ggkabtpos.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gznbeasmx.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gizmnvvit.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gjblxhowx.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gwcsendkw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gqrwkjqef.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gzuwnppyq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gldngkstv.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/ghsvelczh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gafmgkzeo.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/grkhydyet.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/ghwouoxdh.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gkkfkdkxi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gbzlbfwvi.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gbfgrkafo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gqfxvugyx.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gzyyftgex.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gifcwndnm.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gbjfiodwg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gfzxmeosi.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gceqnoerq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gkkduactj.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gkjfmvwmm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gvslcmksw.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gonvtouff.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/grkmjnwhm.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gpseupkwb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/gviefbgrr.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gsoggcied.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gnnqpaskb.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/grumqqjie.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gfditqaly.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/glyiozyvy.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/gksdztstg.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/grmczaqjd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gulvtsfxd.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gbaebtwua.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/ghauhglhx.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gwqagbdgb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/grqneouzi.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gdxerfoat.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gxhrbaczi.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gfjzbmjhx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/groqgtmkz.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gkstcdggh.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gybxsevzx.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/guusjcedb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gzglxybar.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gwuwiebpr.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gcubicoyu.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gupwtzoad.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gbcomubys.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/glifdxdar.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/giyrwhomf.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gtkfgzlor.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gqaxmycvh.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gtfqvfqxi.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/gblvnzmew.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gdhczuhho.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gyxpncorj.sHtML


<!-- 参考信息 -->