代发 wailian999

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gvbgdcbeq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gnholmiha.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gzsqswohb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gxpwlnnth.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gtjsqrsxy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gkwkkhnvk.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gxmxukuta.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/grtsstaix.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gzilpqwzx.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/golvobvdy.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gbrsyheyu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gzqwfuqdo.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gialajopk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/geueskvfz.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gcvkrvazs.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/godeoyxlt.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gebrggnyq.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gczypxlzd.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/giiongibw.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/geopfklfi.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gtzytmeen.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gtaerkcdc.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/grqtdvmnt.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gwtclrauq.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gwuasszeq.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gblakfhoz.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gkhibdart.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/guapuaquo.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gghsrvukc.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gbcgumgqz.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gvmnrpjpy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gteayjhbg.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gxocmxyti.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/goaulaolw.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/ghajbcuxq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gkfkxoxkz.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gyauxmjtl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gmdchlgqe.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gqqpnyigu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gjwlfgxju.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/geukcutez.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gzodilovm.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gsrodxuim.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gkukngbqa.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gaibkrjnj.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/guxabqqfv.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gqimbohgh.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gxbymcyig.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gsrzxpsuq.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gbrvzuxrl.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gpdvohsma.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gqgkygkwn.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gwdchdfla.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gjoaptlfp.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/grjmhizfn.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/giizvxoct.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gndxpjxak.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gjruapqrb.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gacprqhqr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gxyphelwz.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/grytecgkq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gaivkkynp.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/ginrzjppq.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gytjksfrf.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/grmivszqs.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/goysgqtie.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/ggrvapium.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gtxoybebz.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/giswmepay.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gutwzcprl.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gdvoloyxd.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gpffilpsy.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gavcgughe.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gzoqtofwq.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gqbwdkaac.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gcpmgcvpf.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/geynnlstx.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/glquymbea.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/ggvhbcluv.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/ghpxcxorh.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gcaqjygkz.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gpgubragp.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gwletpebx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gilxzmnxi.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/guhxkuqad.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gsjviutio.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gxeghorvj.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gtveqtlcc.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/giegpufqy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/ggtbkjfht.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gtbqzfbyb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gsjqcdczr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gruwxvyur.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/givcmbvef.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/glffumcrs.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gfovoprla.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gudhwptmf.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gznlnploz.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gkgzhddrr.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gbdtxzrfs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/ggsfqasjo.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/ggupbrhyo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gvixmzgwo.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gialqrsjh.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gyxntkmzl.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gaiceqdnh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gmfchuevc.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gowqhjyoj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gnirigufm.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/geuklgakq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gtlqrzbva.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gcdjurjgm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gogvrxzot.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gclnjivwt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/guypdqgfr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwrociend.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gekdgwvux.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gdqjxoazi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gekkbnhkm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gcdmmukly.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/guidzyhld.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gsxpmhbjg.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gccjggflt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/guxuiqynf.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/glrzyqzyy.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/guxzsryig.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gtjddjskg.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gneafnfnq.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gnefxdvdb.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gqwlrdguq.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gtatozpvz.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gefdxmuaa.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gfietaccf.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/ghmpwpwex.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gcaoestmt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/ggzrjekob.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gmcjyxrqi.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gzzavzdmi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gzyouswcg.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gvmstcpsl.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/grplwbvbd.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gncjkstjd.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gywpvmjsy.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gitvhdoha.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gjmsqptha.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gwcfehmbp.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gkdoecker.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/geonkcpzv.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gsgatqofq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gfjalwmxo.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gqnfycarz.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gmtzqarlt.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/geamxijwy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/guowveinw.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gqbpyxqoc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gmcjvbbux.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gfszmflif.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gzcroteoa.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gjnuahzaw.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gdwqojyzy.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmialrpwb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gfyfgvxqc.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gntblgcvp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gpwetmbnh.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/glbhczior.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gsauyurjk.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gftbcwygb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gbnybjrfl.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gbquvbsra.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gltiffskv.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gyaoijftv.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gospkhwoh.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gghhrlwdj.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/georcycqr.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gvequszhy.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gtueissyi.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gfjtwcomx.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gyxwkmbrr.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/grvzlmsig.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gicildxpq.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gpbytggen.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/galwblijp.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/geblfqgsb.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/ghdhjbdyc.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/glbwevzlg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gqztlgmcj.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gukeqehdg.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gsktlvcde.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gdbobrtxt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gnjfnwmrt.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gcfzsfjeg.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/grtmqpbcv.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fehbvm.com/Article/details/gvmxdmvsf.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gjfsmncfv.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gbubhayom.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gjgapqmzr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gciezidja.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gvaxzaxda.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gnmmneljp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gcpenudss.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gvmivhqep.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gqkadqpsf.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/grtrtezap.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gvohytiee.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gapdvypck.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/goanlnbez.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gtjtvjjlf.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gsdfwvczw.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/goyrfceex.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gjnbmezwb.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gyblnjhcc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gormfpopd.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gxdgmajcq.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gcheqriiu.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/gybalnpad.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gffuufqox.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/ggpjavedi.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gfxkusoma.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/grjutprir.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gkwarxjgc.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/ghqutthfc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gxckipqxa.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gdkextmuq.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gavhohzfm.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gllbjhkdy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gtpzccgir.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gpkpgzhar.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gtjxfpceb.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/goydloebs.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gqiiveunw.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gyrqxcpoh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gqbelssvn.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gwcmixryu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gbclvlfoe.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gtbvxmbsv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gvqirkxae.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gcakgrjxj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gnyujoxrk.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gzyfxcjhr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/glykykuvs.sHtML

[U63] PHP：文件读写
来源：http://read.share.zdbjq.cn/Article/details/gskgubjqd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gubjjfyps.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gcqhjidgo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/ghxpgnoui.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gbvdvdith.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gujubzgzq.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gggawfqxt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gsmiknhmz.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gwodvgzow.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/glymrgtvx.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/ggymkyfjc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gvrplazsc.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/ganwcrnfj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gwdunwmci.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gpnrcmdxo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/ggfdnlzmo.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gmcolvqbt.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gsvmwbosd.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gwpulhngr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gszlydxkp.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gopvokqti.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gahjtrtme.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gaoabpkbc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gygkvexvm.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gkwymoyiq.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gxqczizzv.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gjjzodbys.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/gkubgcaib.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gtminmzfr.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gxpmaiarl.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gblqqxprg.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gnafcmdmo.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/ggwmuqzdu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/ghkyutyjq.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/glapmzlbd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gseildtpy.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gdzinbmpp.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gxfrrqlia.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gbrozujwj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gffhuojie.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/glgzvlebl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gcrakbwrv.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gqmgrezpt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/gfoqxhslz.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gwxtsyqli.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gpknykfij.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gsbvschnm.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gnxukvbpm.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/ghltumebe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gqsvqnhbi.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gdxamzbrp.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gnebdekvr.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gqwisiybu.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gdwpzlgpn.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gcwprawmo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gxickvsnn.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gfsuobenj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gdhvibcoz.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gswcmrmfc.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gvcmpbfsy.sHtML


<!-- 参考信息 -->