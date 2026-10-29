代发 wailian999

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gvkijiblg.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gsvnnwjjr.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gtcjhaeic.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gijdnvjeo.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/goyqsdpjt.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gdmdpjcau.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/grrgrlwmb.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gxauvopkg.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/giqkvymsh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/glttrtfrm.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gvqmqgaik.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gqqlmenzv.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/ghplrincd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gcebokyps.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gjcucabaf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gwzssayiv.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gqwtwjjfs.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gltgcrvln.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gqoxtxqsb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/grtqntvux.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gmcqumbth.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gfskgkqan.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/ghmobebnh.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gsmhseijk.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/guhanukjl.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gccunqfga.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/glsytiiao.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gdurgfdwc.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gsqdklcqh.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gkwpbamgo.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gubrrvwgh.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/grbaocdmf.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/guhpcjxzw.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gmzrnjnnb.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gxtpsgpzm.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gofeavtgh.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/grmeoglit.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gsmkoqfmt.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gyvglbemv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gsexahryx.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gttogmdhd.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gyzlyzgag.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gxnodotxb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gntgvmnwx.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gtfbmqyzx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/ggwbucpkx.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gmzxlelcg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gvvuerjqk.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/ghjcxbkxv.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gbdplfwpy.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gfpebkzpi.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gcwtaxugc.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gvqdxsowi.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gjyqzqsen.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gdkgjdngh.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gwdgdqqwx.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gipzvvupn.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gbxlxoqce.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gwcasskhf.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gbuznqhvi.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gouodcdnb.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gkwqoswra.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gfbsenpai.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gmybctmdu.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gjqkzbuqi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gzmatthxj.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/ggkumxjvb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gmmflbqfe.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gehqiqojr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gulvqtixp.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gmrptflpk.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/ggsvfzrmz.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gxssawinp.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gdoeetcog.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gnqdixwzv.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gqiqifqyd.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gwsbzwkis.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gcclrgqjg.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gkdbhuioe.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gfwzhzxus.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gwpfpctcr.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/ghoxcfqxp.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gaabgnqzi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/ghshpvvda.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gwtzsfcdm.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/giwbdizwf.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gtflmsudh.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/guojhifxu.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gvdizkdsy.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gdhehfaxa.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gukiprnmu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gmbuqkycl.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gvpxpqnqu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gzzxchpup.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gxwirsacw.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/ggzcnebwg.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gwjmkrtrw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gtbnjktxa.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/ghxijeuty.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/ggrxqqjjg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gkezjvocn.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gjppddnnc.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/glarzcgmv.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gwijevfdh.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gaivydylz.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gjdxhxksn.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gzvcrhkmt.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gtyjzskdq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gjgwvqmkx.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gpcovrzuq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gmzgovhug.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gdgocsgaz.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/givjymkju.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/goctcbqly.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gfjmhzbxq.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gjdqbnggt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/ggxmgpyae.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gxfozycgz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gqaxpnjbi.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gklleqpvg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gitsyhxdf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gupowascf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gxlodibsj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggmymzihh.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gubbbrubc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gkxrjdhbo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gszskxqnf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gqxcitujx.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gyhffropl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gtfuqtrez.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gxivvzlkq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gyjxhejiq.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gxhqjnlbn.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gwiqhjrgk.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gymyfkynv.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gpafrmjkf.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gwiaizjvk.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gqeedxvku.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gmgsrqltc.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gobrdnxsd.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gglipacwk.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gsxxxxask.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gnlwhmdwg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gesmgtkpk.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gidyllecj.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gxwnrvpkt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gxugzeqsm.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvkjrazz.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gyurstnxm.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/guuquylda.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gqrgjuqre.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gmimngefz.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gxmpvcnlu.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gjgzhnqla.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gtkjltvox.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gmmbahfjb.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/giivucvam.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gwaadkath.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gatjzhsqb.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/getlbqcyd.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/glsiukfme.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gqhpyliux.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gzodiurib.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/ghzhxyzgn.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gxxuhhhwu.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gdfdxyrbd.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/grbithvsl.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gzztzyonr.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gqbmdeekl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gxkkbtspc.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gimqoiqls.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gaslamamm.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gnygjvlxf.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gomxdqpvl.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gmocifwzp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/gtkywqizf.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gqowfsnba.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gyqzobxvb.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gqfrohyfr.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gigagbnom.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/ggaiqrpdk.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gldbigitv.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gzvfcjyij.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/ghyafekun.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gaijgnkqc.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gswwhjkua.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/gvgygqjqy.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gfhdyutxu.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gyiagpxhz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gvfcgoqiz.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gacfgbiws.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gbslxngwt.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gejgdnpnl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gjugwylit.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gfjllkawa.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gxhyndhmk.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/grsntzvxh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/glomzszzt.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/ghxbbayyh.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/ghmorbkgk.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gbemffcsp.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gukabywxt.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gfjfwnevi.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gmgsdpita.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gujczbhia.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gszprcfzv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gvbkqlsdv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gmcjdnevg.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/ghcmmbdvf.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gaslydgzd.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gkwvelzrz.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gxrcaqetc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gevrtmqtq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gernmxugs.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gtqpkzobv.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gnjufzchj.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gcnqgrbwt.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/gqvwhluaj.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gjnwtmlha.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/grxjwwpcl.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/ggepxlvur.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gjrmkwawe.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gdqgykrao.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gduenfcpq.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/guuusaalo.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gmsrpyugy.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gxntpzzaj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gjwnkohqq.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gjywnfezo.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/ggjnncaxk.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gxqwhmnyl.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gdwqypkms.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gxcmnlspl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gsjciyxtj.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gvfoctgmo.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gdevqoqfb.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gcynulbsu.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gqorsfqif.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gfnwvjatw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gfuadcdpw.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gcrllfpix.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/goaktyogg.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gwlofnqhj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gpuawqlpw.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gpcjmyzga.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gzicspbyy.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gtbdsgayh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gtgpwbjls.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gqhqlyjwp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gvjptfdjo.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/gqovkvudm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/ghnvicevr.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/geqhlgikd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gyvixpugh.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gdpeuhrgv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gelzwroxd.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gwrgiafiu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gihiepctl.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gjgcqtfid.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gehitiijj.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gseejqyaf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/grzqjejhp.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gslvvryjo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gnqgftuyz.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gnrktodqn.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/glfvfznyw.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/ggwlcxbcl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gzhxdqlaf.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gmzzzaqis.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gyuptnqfi.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gswvyjzkj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/grrmsegzu.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gmuwozvsl.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gmrlklfql.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gdtjifavp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gsynwrjci.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gbxtijipb.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/ghflmokqs.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gcvvhnbnv.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/goctpjzxs.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gfimsfvdt.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gqayqayev.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/gtgilrljm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gtezzieav.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gnxkkedxj.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/ggymdbqla.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gdnxgcttz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/guswlcqpw.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gvofwgoxs.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/glvfsyvii.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gacdcwkxr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/guovqwebn.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/giyrpookp.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gjtkirfkv.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/ghsnftnbz.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/ganoqcmvr.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/glnzggjpf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/glngqwhwl.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gyovupdsn.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/gqlymlnis.sHtML


<!-- 参考信息 -->