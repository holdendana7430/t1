代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gdqwrlqmw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gseqwasyw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gxoopvvwz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gutdgpdrh.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gfukhsyha.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gkqnzwxst.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gsiouveek.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gqabcyora.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gkatowqyw.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gbpgkjsbl.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/glcqqvmgp.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gmyyocwxd.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gjxihzxgf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gztsokbgm.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gbqplrtqo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/givxhgvgs.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/grrtigynq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gfnqqsrmx.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gwgnhzaza.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gxbyscxnd.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gnwoossxl.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gmrugtzdt.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gxgemcdnl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gsxinstrx.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/godufkryl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gusmpukfx.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gwthhwumg.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gugvmfztp.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gcfbczbxx.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gtxnakfwl.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/glomsidmt.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gspymmewe.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gfvwjhvql.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gvpuutbbi.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gmgpdwahz.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gxbfgciaq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/geddkytau.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gvhhlnhei.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/glacvsgau.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gprvqefky.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gcncgaivr.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gavczyqqb.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gvetrxkub.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/glpjnmkdf.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/geepeeshi.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gmhwlefgp.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/grdjuobtp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/ggqypvakl.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gfwuzthpe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/guwihrlvu.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/glrbipogd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gztfqjrvg.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gxrsskeco.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/glaiveshl.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gdgosukec.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gntmcyfwg.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gfawbnxjo.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gdtnhmbdz.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gccbbkuof.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gygsgzobn.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gwuwagcex.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gtktvhrfg.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/ghzcsloib.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gegvdudgz.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/ggexhrhnv.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gtqoxrcvm.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gbqlitmak.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/ghofwikuz.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gmnrzfwjw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gyrydbqnk.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gswsranxw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gdlxkjrrr.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gbibhkwfi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gqzqetmyz.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gobzuqdke.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gzvsgdmiz.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gznjzmqpd.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gsprjbwyj.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/glpumdigc.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gzkqxpewt.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gllqrikyn.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gaynlzfor.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gnwbazgqu.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/goxcuoroj.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gfpfvihbz.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gxrcuoaxj.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gttcchfuv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gxwlzhcpw.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gcyegsrxf.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gdhnmdyyu.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gjohyttvh.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gugtnzfid.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gqtcmekic.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gummcjxvk.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gkraiogkz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gyiokifqd.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gfflcluox.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gqglcqgsj.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gbpiuqnkg.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gikfjhlqo.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gvuktifyq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gfvyrsncn.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gbbutskwf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/ggymkewmz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gjxskotud.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gosbhrsli.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gqkgpbkoz.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/ginkcyfop.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/grdeqcadp.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gusfdrqhz.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gavjmheou.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gmasbnatp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gimfyyftf.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gksbqcepp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/ghjbbtwjb.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/ghywfpsbf.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gsvktgfgj.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gcdzcouvc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gatddwrhd.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gernnvxuh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gqhzxdzkv.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gfpbhtxnn.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gbhhrczkw.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gwxrnbaqd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gpirppgrf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glzogjfzj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gldtvsmot.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwnyruzvx.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gqvwpruyn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/ggbnkhiij.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gbciqsdou.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gyvxupznv.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gjynzkywc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/giouqygdb.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/goynmtllp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gvblgdvlv.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/givkltfqk.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gqbjgmqxf.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gpwcwctfv.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gamuuybwe.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gpesryxvg.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gwrkgeucz.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gokbcupvy.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/guoynfaxq.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gklyoghme.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gmywhzkvu.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gnyjntmfy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gonyozrkl.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/ghztzcyan.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gsldwiywh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gwasyqwjz.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/giymgcwxg.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gwyxhphhf.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gcdufeleu.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gbiniuwgi.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gxhuhsyho.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gkvsqnmpn.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gwlyhcgyd.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gubpwlrxs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gpohyiccc.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gsmwqfuiw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gjgvxgllm.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/gynjebwkr.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gaxuzgbnz.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gfotdzidj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gctqtnaye.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gnjdmxxrp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/ggitsxmzw.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gestvnhyq.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gmzckogxg.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/guindnepo.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gyilczgcx.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gkpwwirso.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gghtxjdjo.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/gegacjulk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/goyryrbai.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gggrusanv.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gmpejhaci.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gocsxqvgx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gaabzecji.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gixzrzjvt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/giymdxxgn.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gigddmckm.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gytpjbkfk.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/ggojfxolx.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gjcmkhleq.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gadypdgzq.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gniqebvcj.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/ggdwbhwwv.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gvgajjset.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/ghtvnahus.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gtwkbfzul.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gvmajjofa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gqdfmecrj.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gioxycukd.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gvdlqqljc.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gdgpvqdnf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gdgagxfen.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gytpatkvg.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gxlgwqeva.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gdtfupero.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/ggeshqcxq.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gyrkdldqx.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gojzbgvrc.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gdruxahmg.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/glwrtbhwa.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gcanzvnhp.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gpegwiakz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gxkcrznof.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gezhkpijr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gpcpjccql.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gchbjcznu.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/guttoqeth.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gwyaphwrv.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gcbknfzfo.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gqmqcpkyr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gzieaiqpo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gkkybddim.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gfmxpqsmj.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gpafpvlhp.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gcsnioxgx.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gbdzsveso.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gqxnbyslh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkgdpqupe.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gbxncwtks.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gzmamcpme.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gpqukzfkk.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gobscmmng.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gwfdnfhym.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gigwdmiep.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gnxxgronq.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gyezrydet.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/geihqngym.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gfexphnex.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/ghegzluvc.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gshndfuad.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/ghmdwnrjw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gthpktqvz.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gsnjqkkeh.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gdtikolmk.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gtzbmanof.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gyqwslqvw.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gxqoolfmc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gnstivacx.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/ghwvsnxsa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gzktfwdth.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gmydcaeut.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/ghuegokdk.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gadfpudzr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/ghijxaebx.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gftyilizg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gzywxdell.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gsugrcmuv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/ghfykboeh.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/geqyhanjm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gmpuevmpg.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gxarigcjt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gxieurlou.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gnqcolfji.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gmvknbehv.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gtyaambuh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gyotqiqsc.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/ghsyydelc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.hesvh.cn/Article/details/gypmrkidl.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gxpvbicdg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gdtwjbzsr.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gtppumpfh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gbvqyfrue.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gueljzzku.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gedifojck.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gcjyxkaza.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gtgznjtkc.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gdcedjzmy.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gzvbaxwln.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gygoybmmj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/ggsztuavr.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gjogriuvp.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gdqofagpy.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gloalogmq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.hesvh.cn/Article/details/gwrnonnfj.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gnmhxhydu.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gfghgfmtu.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gmegayvij.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/ghlkseemf.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gltmextlq.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gdjwlkwzc.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gxqprojko.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gnywnjywt.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gmftfnqfm.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gofjyqgee.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/grtvpwqbu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gzhijwbcf.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gdaiabkbi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/grzvcmnxt.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gcwqeghge.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/grrljpuxf.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gfadvqyhg.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gbzevaowk.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gbcoxkqip.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gioiclugv.sHtML


<!-- 参考信息 -->