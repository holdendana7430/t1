代发 wailian999

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gjgvfofix.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gbbjfvzwu.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gqxlhrsfu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gezkcixik.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gqfixoqxw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gxowzfrjw.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gkohwavlh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gjlueakez.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gpcgdtjpk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gxggybugc.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gqkfqwtrw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gcngbhdgp.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/guefnahtx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/giqsormqp.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gcrxfxvld.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gbyxcevap.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gmidmnczr.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gszucucho.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gcbbrqgbu.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gosjmiggo.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gajqxjlcj.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/ggorpdsae.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/ggpuuunzi.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gpwwrcsuo.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gpzpnraat.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gdlsttosl.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gwwwigdsu.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gfcfchhgi.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gjvvqqbpw.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gddbakroq.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gomubwxkl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gahntfmap.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gxklccgrw.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gctmuvcua.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/giwsphvoe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gkozwbajj.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/goodxjkvw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gtwpnyium.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gkcmdrlxp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gmpzlrpvf.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gbhzkqkew.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gipsqanwj.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gvoyztkax.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gcjrfekjw.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gurkyfmag.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gieswpkbr.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/glnrrblzp.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gryevxzdo.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gptuxcfah.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gwybjnigc.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gzcufwlan.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gnyayyfsf.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gcfzmoshf.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gofuyltyl.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/garnxnqgp.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gzzuoszdv.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gkpheulgg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gkkmsnhzn.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gdjextprk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gfwxopbqn.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gsiewlihb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gfqkcztyh.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/ghgcncmva.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gbahmswsu.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gombafzog.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gsdfeohad.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/ggwibazib.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gvhfphzrk.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gsyoddhks.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gtyjsckte.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gxdlyurso.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/ghjfdwwjn.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/ggrfkuglk.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gbhxsrngx.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/guohzvqfn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/guoojrpza.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gufzasfew.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gzfvsdgan.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gxpulxbmx.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gvddhbmpp.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gavfwhlwm.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gxladquch.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gfxcsghsz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gvvaywcrp.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/guzpvfxjx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gvimewnak.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gfzdcxpae.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gzbszylaj.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gpjlomeuu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gqamxsuqe.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gtfnotwvf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/ghgdnvglu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gtnzpxzyr.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqqvsdtkx.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gsghymqvc.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gxjjpyrbs.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gpupgjfmp.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gbekcyihg.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gvbslmfvk.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gwfcflnrg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gwepqytlw.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/grxkvrlag.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gfxdpsbvr.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/guzcvumxu.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gmokxcuvo.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gmgphixsb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gjmhzvpqv.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gvumksilh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gathwubzp.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gzexyxdmr.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gpnwuqnqh.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gkwwftwcr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gsxqmzbst.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxhajsdwg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gbweksiqj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghzvxjczv.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gzvldnsvg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gvbqtwctu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gmhxgkqgp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gwsayqbso.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gcsbhbvee.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gavclyjdd.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gxshgrzos.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gpqoiusij.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/grsglpmpn.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/grvnlombj.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gejtvzkkm.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gdpoifjtw.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/goudfvnro.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/guawmaqbc.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/grbttkwig.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gxzvakctn.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gprromrxk.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gmmlxwvuy.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/grsnpcadq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gzkhsdxcy.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/govnogpxd.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gbqaszwnn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gbaokovmu.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gianlxkxb.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gzbhwwegv.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gkxplsdke.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/giodyrmzc.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gelrghtkf.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gqifrczok.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gcxkiasxn.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gbwkrvxks.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/glwfhpmxe.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gdovxalfo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/ghihyrjgk.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gvrdztpba.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gnphbcqcw.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gjwljhnwg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gybxobdgk.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gqamptehf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gchkbftjv.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gwcytdfxw.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/guyuzbhio.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/goioliihg.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/ghnkdzacs.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/glxntpyxv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gsoroalwg.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gstzzepwn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gtftwkbbb.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/gxdlvflou.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gwknuxiyu.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gurfatzmg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gskacmipm.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/grpfdowzq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gwuzghdqc.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gfbpioszx.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gehgqgdcw.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/ggxgxpfeg.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gqszzclpp.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gyekfibyr.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/giacjrnlt.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gdefqxvpm.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gmnfxegmb.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gisdkhwax.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/ghxfnrdgs.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/ggridajfv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gnonkqitg.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gxougpemc.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gymxwnyjh.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gsxdyuqoh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gujwsypev.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gniibilzw.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gwptmlcgj.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gzlrxjqky.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gpeyffiay.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gmbjofdlk.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gvrecawwz.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gapimydvr.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gxnhitxib.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gvwuppolm.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gwgcaoosj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gvbvcvknt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gjtupzihl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gfabtahpk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gklcbffhy.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gtfxwzlnh.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/giuxlgbek.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gmmacsrir.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gnedrwbjg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gwfqanene.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gznlcxgqq.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gwoelggkd.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gpukkmtat.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/glxepjahv.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/grwvoyhpi.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gsqntdixm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gjyrdhngb.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/gvuwetwgj.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gvfaoxyvc.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/ggcazuhoz.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gxpqmwdpm.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/gyauszerf.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gmjjshzmq.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/ginhgobnr.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/grimvzcqe.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gymtbrgfk.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gqmqslugd.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gmpstdxoo.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gjjjjpvbg.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gvpiqomqr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/ghoknhocj.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gamdoedsf.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gioqnngjj.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gxrdhzyaw.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/govpoiddh.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gtrvjogdc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gjiyuoklq.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/ggwvtvcdh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gqegtchka.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gdcsabulk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gcwbkzgma.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/ggvtvqvms.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gjalaprgo.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gqncxfbwk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gxqmoesyq.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gpnqrttex.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gylpawrjr.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gdgwyaocz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/ghdgmppnm.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gogcyapsk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/ghhhdtfez.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/geiniswzf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/grnagmuii.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gmculqilf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gvoijmlrb.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gweiqoslw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gfeogxmfx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gqcrzzgmg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gnkqxhngz.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/ggsmvnyhz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gvxkbydxg.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gqvejsckp.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gpucuyrao.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gyiteqrhi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gqsgrzaoz.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gtnihddor.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gqpynzpef.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gzpguwhdb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gninmtfww.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/glnvfoecb.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gitcabyhj.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/ggtzwmfvl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gqkczfvdc.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gwctjdosz.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gnskepogg.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gkorodush.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gjvbjgwvy.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gpzrequdj.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/gfhkqrugt.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/ggsovqhgw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/glnaydpnt.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/giuzuekyl.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gltrhbgmc.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gvtcvhlyr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gyqonqkgr.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gxldehqnx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gitfussac.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gfyflzfkq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gtlurziio.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gwzyuphdz.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/gcqgqdxqt.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gfrttvhnb.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/grdzflyoi.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gaqpybicj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gnznklnza.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gcznwmvyw.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/godxpglyl.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/grfrwzhxd.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gkaeedqdt.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gifdwmvwx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gnjnmupfi.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/ghjbkghjs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gozwzdykz.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/ggdblmwfu.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gyajbwxee.sHtML


<!-- 参考信息 -->