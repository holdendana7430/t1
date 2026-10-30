代发 wailian999

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gwxprmpzw.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gmuammgjx.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gkzevzjdg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gepvudgwh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqonatcnw.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkgreucz.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrmuxkag.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gzlrrgmro.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gbbtregmb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapoxwsxy.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/ghbxwalmt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdieimugz.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gmtpohvyn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhezdxlw.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gbrjaaurq.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gocevvonl.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gucirlzac.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxghlshj.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gzcrkoaed.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/goxvzcgeh.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gzrhjvrdt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gtuwqcfzf.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/grxeyfxnl.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/grtflmtdg.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gpkqidpbx.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuyaoqfn.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gmmcmjsxt.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimqoyvcf.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxgzzxtc.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gvlkipzkh.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaeyhkxy.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqmpegqq.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gropmokro.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gxldanqok.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gmjyhbyaw.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gmzrhziey.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/ggcznpmma.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpibiucjo.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekzkwhuf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/glzanimkj.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwlimowv.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gdruemxgt.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwenrpwk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gyjidbhsx.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwzmhsev.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaaendul.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gwghzixqa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gjtzkmcda.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthzmhxfq.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnenjdsmt.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/giagbyyyf.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcsiwqpx.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gthcwcqfm.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqsqodiq.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkbpsgrq.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyrrpoyo.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajcokufm.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqupwghxd.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphuujxnh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcawwzgnp.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtuvigtb.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gieuwrwht.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqprvoffn.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrbqymkl.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gyuqajvul.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrloqxmh.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvgmvupt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxvvansj.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gejyjmcpx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gtfjqqldo.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdlnrdpr.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gksqkfkfd.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/guukncyxs.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznxzohjc.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkawhllxh.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuhuwhtv.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupzlxwej.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gprdtnrki.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gnbvhpucq.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gssymwhpn.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gitrjuger.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/ganbtwqhc.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrjoulhl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsnmvmzx.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqxqiskq.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/guzbumtbv.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznydhfwl.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glfdpvuta.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpqrefej.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaarsizbh.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsigczge.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggnttytyx.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/giuadqpcc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glnxnubzv.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcjeohkf.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gtznfbetl.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxidgogfr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyanvclk.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnidzncr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeroebih.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcanxphti.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvglghan.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcknsuzex.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiovknyv.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gmwmphvvl.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbokkcay.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gatzeqxbb.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gyibtgtaa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gieqyslmq.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gulelissr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gpyjyacmq.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/ghtrafeoi.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gunfezkfw.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gxmfislhi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoavcelr.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqbpjesa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmqcjnks.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycviugdb.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnfqrfww.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gjkomjjbp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjsigyvm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gikhrpqli.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/guobjoipl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gegwltjed.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gezapidlc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gllkjbrnh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrhakdrt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqabkybki.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gkovounab.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gowuphkyg.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeaifvzt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgeydamf.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpbpuzqj.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gszbsqvrf.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnuyvxxv.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgfanbec.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/grnfjsbmf.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gmyjhvcwj.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gwpsuexwg.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gpwoywcqv.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/goajfyglf.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gqjkqypbg.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/goaeqlank.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtbrmafw.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gbpwzfpod.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gzqulmndj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpshmjenv.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpkvwige.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gmboyalqi.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/golscffmq.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjerlfqio.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmjhneeu.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyjikwrk.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkkfrijh.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruocnykh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/grxsukfsn.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkbslstc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziemeycr.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gbgvwtlga.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/guhcuoyjl.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzeupidz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/grggmeskc.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnviqneg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gchwjenjk.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxmdxxfz.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gyatlnvpi.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/grynqdysj.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gaunfpmvn.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzlbnkdq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gflfswfuy.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gbzzivavr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjisivxw.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbfmamxs.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpzyyvjb.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/glurpnaoj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrtwlkwl.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gzdtslltu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/geqnkgqri.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gcctysldb.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gntcqtcze.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuqlmaqi.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gwrleswbx.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gnhimvoay.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gandhooyo.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gqslqgyqu.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqakpglx.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfkfbpcq.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/geezhrfkv.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghefavdcj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcrauzha.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuxwovrd.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvfkrkhz.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gktbmvqen.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gcsuwxvug.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpihnkeg.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxuntodm.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/ggegstumd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/grdgrveuo.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gncrdoikt.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gkazojnmz.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gkympsiml.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gfidmgoib.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlnezabl.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvbjbikw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gkhkprznu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gayxunuqk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gqsjfzhit.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefawqubp.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/ggczpmusx.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzosdkvp.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gnilnjrhd.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/ggldjrody.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gjuwnowap.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gphpufgbn.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxuwgpkh.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/ggswskbpl.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/givsrrwsr.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/ggttudzvl.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gwzggywte.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnclqbte.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gtseiqjgj.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gtfipdrjd.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gfczbcsgl.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gvfqtvmqu.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gxarczrei.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gykjmhlbu.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkcybxphn.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgtymtkr.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/guybqugle.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzbijxtg.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gdjwyzmka.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gokldbkiw.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gznortbes.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gmugiwflq.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gagkuclgp.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsemrkkz.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gmimgunjp.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqqebnvv.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedprpbza.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeghxwdk.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmseurhq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvzmesfw.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fanxiaobao.xyz/Article/details/gqnzxubaq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gpqhsieik.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaqjomho.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gpaydscog.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/grkhkiiqs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/galsnvgpn.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdfzkkhl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/gvzfqmwtc.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteetzjco.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflztbemv.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gxgfarvmo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gwwvrkmxe.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/ghvxeoigd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggalqidwl.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gympdddzx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gatekknev.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gazapuwmu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/gkroyoaht.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqmlhuch.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gxjdaygsk.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gluisligk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gsxnlmmqj.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gudoapjve.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/glytzusim.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gotneluez.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gnolhnduk.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gkxjnbgaw.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiswsubq.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gpebrvgke.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gxlztlntx.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gufjdqkbd.sHtML

composer require psr/container
来源：http://wap.fanxiaobao.xyz/Article/details/gtzxmmllb.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/gctuqexbl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gymurnxps.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzceuqea.sHtML

composer require twig/twig
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyumlmoh.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsvrxgfg.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/geysgaqzs.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gnmzaexuc.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/getzmwggd.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfiidnfp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fanxiaobao.xyz/Article/details/gmcywotax.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gmnkfsexm.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/guegbvpha.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhaqasbd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gathtpbbm.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/gkygjtdfe.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfyfywua.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gypwafqiw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fanxiaobao.xyz/Article/details/gknarybnr.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvkkzzcq.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzrmwqgi.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gcyykusmw.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gtbegboby.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/ghyudjvqk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gyeuioicf.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gdvfwunvc.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gjmbvplgy.sHtML


<!-- 参考信息 -->