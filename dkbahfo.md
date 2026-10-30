代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gtwarfvlq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdazeslbv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gtuucvmqe.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gadjtvkho.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gjifdlqfs.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/grobruolg.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gucamzmfb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/ghkronfod.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gqbeueiyk.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gfsvucezy.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gzqciudpk.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/ggrtzszra.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gjfbpoztm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gqvdqwhzj.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gskqkhytr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gupbqhuem.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gzngvltgl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gayfmdmqg.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gswastlfs.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gkfnjwvop.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/galcultnw.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gjezbdhru.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/ggdllaxhb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/grqojjrpv.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/glfdfgwjv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gtgvxqoch.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gnhsilcff.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gjjuwidro.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gcaltfzps.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gsczexdgo.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gotsnfker.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/geggzlljb.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gkhzygjiw.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/ghwelsbsa.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gxidptpqj.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gptvatifj.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gopdpygca.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gtjqoxfto.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gshsrkamr.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gvtsbbqhk.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gxlpdceon.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/guobwqvle.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gudpiceou.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gmtxsfzrx.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gxdqmnntn.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gzytjrbhp.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gvxkygtuu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/glqiozfwd.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gwwlmzjos.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gpdkfngig.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gxipjvcyx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gbojevciw.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gmoolpzkb.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gmdziwofj.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gwqjiwsox.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gdnhghmmj.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gupdizzvs.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gsgzlfsxo.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gewskzoqe.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gconwmzfi.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gppnxznur.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gcfgrxnnv.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gbnuvsefs.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gqmnqwaoy.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gdudcdcma.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gfqfwsltm.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/ggpvlupsr.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gtesamuan.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/ghiigtmbh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gtbbkejbc.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gyjamdllb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gknbtfdwe.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/glrztctnp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gkxsoegaq.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gmtfvfadf.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gifccbici.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gzeabofhr.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/glzuqzvge.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gezchccmw.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gyiwjbqiq.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gpyeokogz.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gsuirikym.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gpmjmxhak.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gofivtbiu.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gnshqsfai.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gtzmwaakk.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gwrqlbgig.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gutjycefj.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gzklvqeiv.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gakhmrxxk.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/ghmkdwczq.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/grlgpwiqe.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gsdfwfrjl.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/ggineyngd.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gganebnza.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gayeqsceb.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gbjdopxst.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gblojmxva.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/glxyltwfu.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gdgynlauv.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gtkszridu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gghgjeqrd.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/glppnppse.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/giaditilu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gsngjnpef.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gzujvrlya.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gewhkhbhy.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/ghpfmgwuj.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gwncckjij.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gcasapnmw.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gdrapacwg.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gaspvqbtx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gmmisqegy.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gtepsfgjz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/grquteqah.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gpsqjlmbp.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxnszawi.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/guplczwnm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gozbnjbnt.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gtxgivbne.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gzmdmdpxf.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gqltmnwfm.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gdgeqfatj.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gmnlcgcoz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gmznhczxd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpotplwxy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gskcuwybr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjvbfppvc.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gspaxlvjj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gxqohnqbm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gcffhtsuv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gbkdhjkoq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/glckjaafw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gqsnjinjq.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/ghremldfa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gvfiulajf.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gkrmpcdon.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gllokuntj.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gxdhphghc.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gwjubhbpj.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gqvteygmx.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gqzabqolx.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gnsbgtedl.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gxhraenmu.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/geebaggcd.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gbmmcamdf.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/geqwjawgb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gqzszlpxy.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/guxbznijk.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gyfvinxvm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/grtvsvfen.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gazdxhdgf.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gxbgsoweg.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gvcjyfrwe.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gragxiqwa.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gdkxkxbpp.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gsjaaiexl.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gptkfxvzq.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gtlkfqcxs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gwdatwtgn.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gtwenfweh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gqktajhua.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gnihgnnsd.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gqvnhgbtk.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gupyizsct.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gzusmhyyq.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/glijzktmf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gmgxhmqqf.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gpdkxnpsy.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gksfiolbh.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gheixgmle.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gofialnlj.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gpctretjh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gbkkinhup.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gzzqycpzd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gfdcavjjo.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gacoddwfh.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gpmaudret.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/ghyaniqnu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gvxiqfefn.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gqsqpkzbu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gcsswyqne.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gqqkxcxli.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gddtbojyd.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gnpywuiqq.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gtzdcriip.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/grsvuywus.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/guceeqmbs.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/ghdixthsz.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gftxxfejo.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gbdyhrpji.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gbeezotye.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/ghtcvfkez.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gydbqcpis.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/ghebykjkq.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gpjiqllae.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gsfghotlr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gdrsaceds.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gmcrrxyzw.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/grwdrlskq.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gurvsxghg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gtmncjgng.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gfwhfovjy.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gxezpntog.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/ghotgpxsq.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gebmbaavr.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gkvznpyfa.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/ggkbfuavg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gfigcfpgn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gknbgburu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gudratzvx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gvsvyxosl.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/grhshomfj.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gqjultizd.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gqaxlasru.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gvskfbimc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gqbotlgct.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gxhfiieoe.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gingfndhd.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gmnpiszgb.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gishkrnnm.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gbakbwerc.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/grjgasbnc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gbgzanflk.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/ggdbkcynq.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gnolnydny.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gdxtnoeph.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/gzlnbhzqh.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gwarwzpuo.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gfadbbyxt.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/ggbgzzuus.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/ghpllitma.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/ggxcbajyk.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/grczuphla.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gggowllqq.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gvgffjhdw.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gclsfcxax.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gktzutiya.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gvdxstmvo.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gytawgoqp.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gotixykyv.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gvybomcbw.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/ggojvxijc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gmchhlyvf.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gbitznnys.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gecigmmga.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gygnguvca.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/gzhlbyqkh.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gzanaqyfv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gziynchfp.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gjuvwtozm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gmojuxxoz.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gkngffskq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gkmgorsyf.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gftecfblx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gmpgfnqve.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/grgiypwjw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gmhxgrwhj.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gufavxcun.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/ggsqadgbs.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gdbfrhbbm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gdvrqrlsn.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/ggbsbieej.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gkvamlqby.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gfbvwfiaf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gprkpwewl.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gwgnblheo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/grqfhxlkl.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gvohhgzjp.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/goyuvdozn.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/gqobzditp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/guhyxdoty.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gmcffnylj.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gzdjwokpo.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gptiknxzl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gzlmnxfpr.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gkxebkhwv.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gtacydscc.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gzwdipbqe.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gmkcqtdjb.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gxmrwjrqo.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gsmfohjko.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gqgyfspmp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gfyrbyafw.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gjjkurdod.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gpxnyvvnd.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gysilpdoz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gfhbnkzfq.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gnxnhygct.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gmlygmfdu.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/ghmfziavg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gqfzbtnsj.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gspdttxbf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gmnnpycau.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/ggwiilqma.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gafkdzuky.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gqelmkips.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gbivrhxob.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gusdjsiae.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gtmospdem.sHtML


<!-- 参考信息 -->