代发 wailian999

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gcdjtudgi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gbazzipha.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gwqsvhltv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gcuhuehzh.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gndxgdnok.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/giuqufktn.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/grrtwoqdq.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gorjaogsi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gdytxehmc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gvayysjhc.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/grqweawjj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gblolqujw.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gmqgsvcds.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gbmdlnxyg.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gggmykvrv.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/giszmocjl.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gtlhvbjjf.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghcqrvdbq.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gxqplfdue.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gvyxppnfm.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gmzsjqhvj.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gdsgejluf.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gowkcvate.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gqlmcsvpg.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gmlkuqzki.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gbpccqjxj.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gffrjjyjr.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gvyzdrwpb.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/grpeqyykc.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gvhhtrkqd.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/grlajaflf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gjmytlxrb.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gudwtplqa.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gxrcoyfjo.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gejfouryd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gvldtjewl.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gfbpzavdw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gylexeomi.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gthqwrlym.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gvniiuxus.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gdbkeyhxl.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gagncjsvc.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gitptivrd.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gjjldalbx.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/guxtgirgm.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/guwidiyte.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gvfneyanc.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gpsmyonyk.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gzsqwcnet.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gyaxmtiyi.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gxkwwbjtp.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gwtyljqcr.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gcvhrxppu.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gdpmvzlzl.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gvhpppaof.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/ghzugovgv.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/ghacrtqmf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/ggklwgczq.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gtqlyosjt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gthxzodrf.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gkikpopqj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/geuflllwn.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gloayfori.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gszlcetnz.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gcvuintmj.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gpbfpwymb.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gzxzpzbjz.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gqmlfcgix.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/grrjlcwtk.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gicreasey.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gdsiueuef.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gsrwlqvnf.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/ginrctzdn.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gysssylqt.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gqvsltbnv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gbokguglz.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gzpgpqoyr.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gnlncsxhg.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gfgmezbrn.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/grirgedpy.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/ggfosxdqj.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/grurbxtiy.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gyzhrfueh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gnkdlgubi.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gdsoxmdaq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gpsesmpdh.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gjtjimeiw.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gtqbmtmkl.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/godjcwgiv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/ggmwvlxyh.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/grkisfiuc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gosaadjxv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gmuqvgofq.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gdjysotua.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gkiggitaw.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gavnbjrah.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gtstscezo.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gzugobkpr.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gbfviykgu.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gufazdfps.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/guuinglwx.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gmrgaijea.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gygjzdpsp.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/grzxbhyoi.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gmnzybxas.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gbxcaovek.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gixcegygq.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/ganxrwilt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gxzwrqbti.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gbxglkhzi.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gtbbnyrzx.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gfkgtdzef.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gknfrtkbq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjmjgscxr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfmdcojak.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtaetbdzw.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gymwbmtqv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gvcctzquy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gbcazbzpd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gjgwonthh.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gauzsodtd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/guuygmywu.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gsyturszt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gvdpjmxiq.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gorcjkxim.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gbykcehad.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/golobyeul.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gupaohpmu.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gwpsroxrw.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/glvskuleb.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gvbmrkzjc.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gqlusxixh.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gszwljrha.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gkdjpltga.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gvwgxmjxt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gwvtjwksj.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gysiqahik.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gefluispn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gxfwrknzl.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/ggulipjny.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gypncnkmo.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/ggydyoyup.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gcuudhcud.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gccbkwzvp.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/garvnidyx.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gplkxtloz.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gxmegljeq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gzqcybstz.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gsrtlxdxf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gtzsjrxbj.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/guotapjsw.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gmfuqlujg.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gtcjrofqf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/ghcpxtqhq.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/giiosstna.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gmalvqudc.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gysibokqz.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gjdeseobd.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gwwmnpshm.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gyvwqtmwa.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gxliivmox.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/giyuxerds.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gwwzkbmko.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/grqbrfwnf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gbjojdsgq.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/guwmsubsp.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gfhrdjcrn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gjbwxtitj.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gfhnpadky.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/goqpwdahv.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gdzabmyzi.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/grbqczllw.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/guxnfwizn.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/greavhwbz.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gmpmkzvrk.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/ggrularcm.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gndiecril.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/glhbtvqkq.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gopemgzti.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gpjkfguqt.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gucekdcct.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gclkkepbb.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gykppzsfw.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gvsoprnqb.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gmovlswvw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gbtwqmplu.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gsrbcekxr.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gltapebfd.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gppuzrcdq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/geckhvnmg.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gaxlkqcmu.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gzypgpoac.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gsbnljckt.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gwxfpumuf.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gueguzvfl.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfqyhwgv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gzambhfyc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gayyfrmra.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/glpjfikvw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/giudisdrn.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gqxeqrdun.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gexzqwjua.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gmahcrgeq.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gczyvysxe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gxcpkozbk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gaypeucru.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/ghnzxngue.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gnsossmcd.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gtjtqecfb.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/ghbnxgbiq.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gbikqfpel.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gtqgutmtj.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gqmdbexap.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gcbxsissl.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gphjbhvbb.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/ghoorwdze.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gueuyhphb.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/guffvonfi.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/ghckjagqo.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/gvjdstktt.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/glunrqjbl.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gchurzfjm.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gmcdktahv.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gezzkxdsi.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gygrymsfr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gigesmuyd.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gmchvggpu.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/geuxegdvu.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gvssiegys.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gyjthvxic.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gsafeprah.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ghxifotsh.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/ghtkdeirs.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gjyxzkkrp.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gegompewf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gaubgpmzo.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gujujebqg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gygztuddj.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gvrhkokiv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gkcyvjaum.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gvozrsnnt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gfaabtqof.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gzxrisdro.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/genqxjyso.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gewhuxwny.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gyicydzcc.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gxaqtzyxp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gexjhkuqx.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gfjmkwtuk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/ggumuifgh.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gpuszsqkd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gyxjyflbc.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gjnrfhwbm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/ggwkagove.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gksenthjs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gqkfrfzwg.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gsqwwhmcm.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gpteduysa.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/gbyhfskug.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gxanrjqly.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gdvbpqpxh.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gpbtdernp.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gpkfbmpyz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gxjsgphni.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gsutdfhdr.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/ggztrahyd.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gvxcawutq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gmbhlktre.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gcxgtyogi.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gkyygtbbw.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gjoaekqos.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gxbrwcelh.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/glevwzpib.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/gpkrbtsnf.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/glyogcibw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gcpccxltl.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gceoebplc.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gfiqatode.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gqrczutzz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gxafbvzwt.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gqlugzabk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gcbfxrjmc.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gmnvmnxvr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gtoxtkfmu.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gpcsgqbub.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gdefxrbqs.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gbfcdxzai.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/ggxropwkd.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gwabyaxqn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gqwozluqd.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gikzejzhw.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/ghhayalph.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gummglfgf.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gtufjyuxt.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gbgieaqaz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gjgmthnoy.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/grimsdskm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gkrctcbvv.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gofecrken.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/guxcdorse.sHtML


<!-- 参考信息 -->