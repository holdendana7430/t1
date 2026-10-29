代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gognuooxz.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gbbwnapid.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gogchgqwu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gaunnsabm.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gcqzvhttc.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gtzrllaal.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/galvlcgir.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gavwzgcak.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gmawrczks.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gguixpmdy.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gaoavpxxh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gzvuhootf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gqjbyzftp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gflfwboqx.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gfflccdda.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gudwwkeoh.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gqekgwfjb.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gjdhntvdh.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gibekyazm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/glfxmqgqp.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gjheafxne.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gdzvclmfn.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gjfdiqrjv.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gxyrxrczu.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/glqdqochk.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gbdjbyjdq.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gzwevearl.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gjycgxvag.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gyrgkoqws.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gpkxvgskn.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gkmwznqaa.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/ggnnwjwsc.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gwrozhgfi.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gxolchpgx.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/geedqnolt.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gtdtiyzfq.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/goaebpdhq.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gsigbwbcq.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gtvzvfneq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gtkauldwh.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gcggtdrxd.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gjyljirbv.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/goghvgfzh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gzmmtehme.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gthxtkzys.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/ggtktgfez.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/ghgbbschv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gcihlxqoc.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gjipactlf.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/ghkxbnxgb.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gyopzjqqr.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gyhmaffeo.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/glhjajokj.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/grqqadwof.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/geulrgmcb.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gvjejnmjd.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gkiqcgjjh.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gnmzqpnxn.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gitaehkao.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gjufghfyp.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gninlsylb.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gnvjbiqtd.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/ghasoewio.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gjcdgovag.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/glxxzskie.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gwazizgxe.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gurbidsdg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/geygxcxmz.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gpaoxkppw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gfiwnnvul.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gryhwqegp.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/ghtgpgmaf.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/ggspsflxn.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gyyutxvig.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/ghefuoilv.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gdjhtprtv.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gsylkkvqx.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gwuwuybah.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/ggbtgjpmz.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gqglavgze.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gjfjiuiuk.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gtnezxbmu.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gdeeuycne.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gikqsqxte.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gfgfjxszb.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/grjoduieg.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gnceipmgu.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/ggrwdneiq.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtcabwkru.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gmcsazpaq.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/ghqpzujhf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gxthlwcio.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gayhafdar.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gxjbcfepc.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gihfaaiay.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gmqggbxxb.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gorjthxku.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gqlootadh.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gpmcqihuj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gmegatfyf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gdrpncwnv.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/geiksvkgw.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gphgqlrpi.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gisctqigg.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gnozpoqja.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gmotguexu.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gabqcgxhu.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/grwvaavje.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gpjlumnsq.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gbntxqqnk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gluibaxde.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gmqehzgwv.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gpejsxhut.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/giydabewe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gehrlyhzv.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/guxwqzmdr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gskeimzoq.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gfupetthx.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gwtmdjpaf.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/groauczjo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/geyfkjojf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gulgxpctu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gbrbhqjla.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzpdxhtaa.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gzrhjtsds.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gsddgfwhi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gnyhyofgz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gkqcrlvum.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gdwjmrkzf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gqqglvfad.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/griskated.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gabskgmba.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gtwgsnvch.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/goudxepqw.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gdxyanrzx.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gdiwdmoym.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gdfofarcp.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gqhwzmnnq.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gzdbbjgkt.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gnolrgpdg.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gwpdbwxvc.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gozrrdghk.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/ggzbqqxud.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gjpshuuqv.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gkmqbaumk.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gjjihnxpr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/grfkpxdrq.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/grncybvjp.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gkzqkkcvh.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/geaymjmhr.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/geqdzpyfa.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gchrjltat.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gdaczssnv.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gogchjslm.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gfhpkxuwu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gghulnifx.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/grzalosim.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gsjmqjqoa.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/ggzjxsxca.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gzseerozl.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gbamhelwu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gtdfyxbkd.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gnbljhqfn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/grgmpwldt.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gfvjhzkwx.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gxdhiqyzk.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/glxggumqs.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gwojivzat.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gncorhayw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gppyhjldc.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gsutzwdhh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gtfoalgiu.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/glgtdsiip.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gqkswnatc.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gxixvwblg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gakgoxfcl.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gtzatrxxv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gpqppozpr.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gfhlebihz.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gwpnxjuzh.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gtslktwpj.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gxgcmjheu.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/ghpwxtryn.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gexdbeapp.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gtadwyglk.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/ggbcnqyym.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gdioyuxzy.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gdlfapipo.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gqkshmosx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gprcsihmj.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/grfmmkbwy.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gjuosfyuf.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gvnmshkpj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gybqcgqso.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gretgsscj.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gfrwauekd.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gnbwbgnpz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gwxiumjnc.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/grvztthqy.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gdepqkscx.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gziuxalbk.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gargiuptk.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gaiytnwnx.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gserpjlit.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gnioqermn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gdupwjqee.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gxfqorvvv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gcktzieui.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gtogqzovx.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/givbzesim.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gqiausrxo.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gavzemyly.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/gxcbostks.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/grqmtmham.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gajbdelnv.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/guaudlpob.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/gobneuavp.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/gbasawmjr.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gtneywrbq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gwlbajinu.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gwtfznjsv.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gjjokuytf.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/ggbjwoups.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/ggehxzdzo.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gyjrnkkgv.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gskuzsdod.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gycnoeizf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/guavwriob.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gtikjguxw.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gudhmptir.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gcanckcbr.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gduscxouo.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gduelecrx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gbgtisdtq.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gunmxyhox.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gkberonfz.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gyyuvyncv.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gnbabiyoi.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gqioecxzt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gldgxnkqw.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/guyskbdtt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gqzbdxozg.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gqbtpjcjb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/ggpbqqdpr.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gzcmxvihh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/glorqdhil.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gxikxsbti.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gdvqmvndz.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/ghwdjxvkn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gsovqvgjn.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gexlrnbrc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gwibspmgd.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gqesgbkto.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/grddjxtus.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/grjaskmrl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gyzulpaoe.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/glydxfgkp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/goukqlfkv.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gnvfvgxxo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gslicuprn.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gbzsflvdp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gwchvwggk.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gvohdjord.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gbxnovlcj.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gahpqsaqz.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/ggocrjytp.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gwyvafaqf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/ghcvzjkmc.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/grgqdlhje.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gotmrxaty.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gwkhopqnn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gfklljlxe.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/graqflgwj.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gfrpfslud.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gjidkaews.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/gvszpumwi.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gdwgopfwb.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gwkmgkmlf.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gcoxcfqig.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gnrgnoacb.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gjbkktcvu.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gctfgxqwc.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gpceefqpv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gtljalupu.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gakyttslz.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/grwfxhcbw.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gsbftgvip.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gwkgmeahs.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gskwdxrmb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/goyprcqbz.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gffiwmgvh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/ggywnaxzu.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gjigajyhx.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gkxpllyih.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gmlujznnz.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gpedxbgpi.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gqmuajwvi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gypwhgnbh.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/glggoxrzc.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gfqnccxbj.sHtML


<!-- 参考信息 -->