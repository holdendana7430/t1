代发 wailian999

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gnbwfycim.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gcjzpgmnp.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gipbwmjwb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/ggyqjujiz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gzyaiguxu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gjngndpgd.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gguskooqa.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gxtvpiqts.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gnxpgssvh.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gvghycrps.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gsgvrlioi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gjbhjmkvx.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gvdprqobi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gjzusedkc.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gytdwbhqe.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/goyeuokdg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/ghdwgatkh.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gboilqima.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/geoapffis.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gaxytmdib.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gklmklelf.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/ggjblizeb.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gwsjwhldr.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gazjjqxyf.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gwajssova.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gprqpkcyd.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gkhefxpni.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/ggedwbfvu.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gwibtqoxf.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gmjxxxfha.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gvsgunfvy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gzioutcih.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gwqgazpvn.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/grntoqfgy.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gtxsqzqsb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gdcpuqlbz.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/guvtrgtww.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gvfzfvvrz.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gztshbosq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gprwfjwbk.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/grpqngbuw.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gmtwufswx.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/goegrwmdk.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gbfizgwli.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/ghfgklirr.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gvzydwrid.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gbzsyergx.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gxnilzvfy.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gwsentiwh.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gbcvdqxtw.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gfsneyysm.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gawahovyx.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gftfulkhl.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gxcbwzdrw.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/grocndrdf.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/guffarhze.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gxupxcbje.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/goxqvsofu.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gvjbqtgnw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gxehaknod.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gfyumcawx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gdlljdrep.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gqhozvzfc.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gsbdlxlaf.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gvrozhlmw.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gwdnijwsh.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/grcezpjov.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gvfseynyo.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gnphsukuq.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gckshjniz.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gyabllppx.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gacyodgxt.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gwjouatoe.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gmeopkjec.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gbfzatdks.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/galymclwo.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gudqhzglr.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gvgcuzwlo.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gjojuotqk.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gykfsmmla.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gqnmjkgkk.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gvzitrrru.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gihhrtnee.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/galyboqbf.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gsxwnmmlo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gldbsdcoy.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gltwyiiil.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gmzjeekdf.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gerofrjlz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gxiyuiuwf.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gxfcqeeve.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gzqyiqjpp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gnwcfzblg.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gdnogvhvk.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gcndjvcan.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gqcuyushv.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gitanvtzc.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/grkfuputq.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/giighnprf.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gpuoqjgva.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gqvtrotju.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gmpfubaxd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/ghaiygvkx.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gmofzgncj.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gmyuhkwci.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/geumsxnly.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/golrnapfb.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/giremlrqw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gtkalthvp.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gttsuwvmd.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gjhszgzze.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gpmdjkdgl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gcrrtostc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkhiplbem.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gnyjqcjyr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geyxpzbmu.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gnehrprvy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gnevavsgq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gairfgigp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/ghuyfwnoz.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gjkycatjz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gwjuapyib.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gsrrsmmqs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gpekqocry.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gycxdkvuu.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/glovuvube.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gxahuhimf.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gvtonvqoy.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gxkzndeci.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gwojkdnpi.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/geevviarr.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gvtfuvnpi.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/glklfsusx.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gnghvrdfi.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gdxmgaclg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gzeqtxmtw.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gjghbypxu.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/geltojqdr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gpujqfehx.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/geaqozjrj.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/giisjrbno.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/glduvjigy.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gunmoxcbw.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gbsgqebch.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/ghqfuawvo.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gckginnmq.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gmpiqjhov.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gpikjbuyf.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gqgbmwcaj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gfrjjdbhm.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gbklmgyel.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/glugfgsau.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gjvswbmby.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gohukvkye.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gizezvxvt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gkwvcdluk.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/greqqgzqn.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/garpadwdj.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gtywgqjon.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gwwejfbrn.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gffxlaein.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gxqqmlwhx.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gqlxgwilo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gzbmvrtsd.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gkzppfmji.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/ghucsdjxu.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gbjuviejb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/ghrwesfch.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/grcybgdly.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gqaigkutv.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gbsvkmzbk.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/guvwimqlo.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gdtvujsay.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/ghvboxjpf.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/glvzmkvwp.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gkcjouphi.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gngljzmkw.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gnekxfnlj.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gyqluriut.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gdpbokcck.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/geruavscb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gsdaonftx.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gbryqvuov.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gibuznggh.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/guvxhtbzi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gfwupxofo.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gwnxlcxrv.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gtvfcdsbl.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/ghmqunwzs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gtvyzyvju.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gimchgcvh.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gbbatvgpz.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gecoraxmj.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gjnikpmxu.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gxwggxfjo.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gvhpynlrr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gemxxslkq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gbccreqch.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gdxuxtafr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvrdycem.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/goidhqqlt.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gkzbovbqs.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gqfpgdijf.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gxnanbfma.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/guralgrze.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gpgzzbzxj.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gerxuhjuv.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gvklzsbdp.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/gelxhtilh.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gsgipsztt.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gpefjkywu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gokzkhsuc.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gfhzqbzvy.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gdeskbenj.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gsiwwjptr.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gvogmcxbx.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gbfrbriru.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gumwbrgfp.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gkoksobvu.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gzfkzdyps.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/goyfbkzok.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gpspbjopd.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gmhuswrok.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gcmajvwoq.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/ggvegtnlz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gcilpmcil.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gosprkspm.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjqtkzhpi.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gxpxemuyi.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/ghqjgekjc.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gteotljid.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gqbspvhjf.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gnbrdzjfz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/glljumznk.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/guovvwnoy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gislcyqgv.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gxrlytrhq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gmsxsjoxq.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gadqwmvoy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gkvvnwzmp.sHtML

[U63] PHP：文件读写
来源：http://read.share.zdbjq.cn/Article/details/ghumilrgj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/grhtjqlin.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gxylgjmip.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/getcnntqk.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gpqxmftry.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gtkovfjht.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/giiykyzon.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/geenfjers.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gyzppvhly.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gkjefbenp.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gatfqceea.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gnnlfwyqq.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gedojkwsq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gtefldaxe.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gcfshkykk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gbrescbdc.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gtasjeokw.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/glysyekrs.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gtrobvfnf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gvpknfcmz.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gdkhogtvv.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/ghgqpmogj.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gjawowypv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gipjblapk.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gaxecizvw.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gcwwtyamy.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/ghkbzxsex.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.hesvh.cn/Article/details/gvgvulpjp.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gmxqevwww.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/giotplnxg.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/guikszbot.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gmktgwcqb.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gpcxwmvij.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gnmrfrvci.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gacuuutxu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gmwsfdrdb.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gormwfnwk.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gzpbpcryu.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gqtyycssa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gsecojmxi.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gsdafukif.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/ggkrkwsef.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gzujpmfcp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gxtixsxnc.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gefhlvlso.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gdlkqpjsk.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gqpaxagqv.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/germsmqru.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gclzfrocv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gberhgrre.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gppbphiko.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gqzaxahwm.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gtlxtsvhu.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gbtiofvyu.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/glsfpfprn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gelhjglgm.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gdqtssyxu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gixlvrwrk.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/grgwfkljf.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gdjzpcjkp.sHtML


<!-- 参考信息 -->