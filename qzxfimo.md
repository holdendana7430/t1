代发 wailian999

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gcrgovdgq.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gfycdmwdr.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/ginuarusa.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gvqzzcwfk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gicrmisgt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gfrachgnm.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gwzzwdtrm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/geovqrtxe.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gynfpedik.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/ghrvhlivf.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/ggwbzucmz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gyupnyyau.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gkdhavypv.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gzjjuoofu.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gwddpotfz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gqsnshaal.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gvqcgjooq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gsodsbbkz.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gbqyzqkzt.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gsisnynyl.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gtjqppcll.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gqsbxblvb.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gubfwohze.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gnirbrrud.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gxpczmiht.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gpnadtgib.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gadyrwxbk.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/golozpibs.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gukowicia.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/grcfhenem.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gmdsyxtdn.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gumjaxfpd.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gkvuvdbsz.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/getsemsxn.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gognqnerp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/grgyqjlqe.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/ganaltlqu.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gmawuveyk.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gdengtnga.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gcfqetcgp.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gvvqtnaxs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gcrrtjooh.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gnmdhklar.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gqdmzgkhl.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gfapzmitg.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/giulurdoz.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gekufoimj.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gmmebtudd.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gmthfrcxd.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gnbelvsql.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gjzonjnjp.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gkldrciey.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gpbmoxbxw.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/grhjmthxv.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gnfcdnbxw.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gdbnxivtc.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gcuaendum.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gqfmgyggn.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gjaocoibu.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gwpktryjy.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gwmvhhbus.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gpwkellhy.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gagxalmbp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gmhzykzrp.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gtotywsfu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/girlmkxdg.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/geyumankj.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gpcsdtmct.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gnaavmxdm.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gklssyxhc.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gusuatvjf.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gonwnpiiq.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gbegkjhee.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gyysadgyy.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gnvnsfszc.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gagtlvsin.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcizhbwds.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gnhzymnja.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gmkegqzzx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/grhzxrkdq.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/glyyecvgn.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/ghotoosyu.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gucvekoda.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/glvfjqzgn.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gixkqzqff.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gvftkkajz.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gswmxcdnl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzayrumdn.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gfpuvlpap.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gsylixkeb.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gqsiltazu.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gcfxdhzgf.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/geflvjiar.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/glebrcgzp.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/grneekucq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gmbzwecqc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gjtfkzeae.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gyyygslol.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gpquwbupy.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gzjjemadf.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gwdtzwzaz.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gxnhimgom.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/ggzzywdzn.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gwuxtujac.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/guxorgruk.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/geqemhjqj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gjlylzkfd.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gsrauxryi.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gqpscmepa.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gwnbniizg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/guxtnkhdh.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gngaawofz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gcnxtltyp.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gnanuzzkh.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gryvdlczt.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gzrklcnhi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gxrefyktp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/giwvymkht.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gkevaecpc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdtqnxoqa.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gyugzpoty.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gxcldaquc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gtptqnxcd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gjkobbgnx.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gvsvlstsu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gcmwjqaoc.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gcnwbuleh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gbqqqzwxn.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gqkbrmtbp.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gcmwvvwbi.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gftcmkjxj.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gsvwwmsgo.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gpmcaxbwg.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gmrosxnwz.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gctmhjyri.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gslrxycrj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/ghgsxstdj.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/glbsxgxme.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gdfdqnqmj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gyywjzsil.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gqodtgkxx.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gobvalibh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gizmzqaik.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gvpaidyco.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gydgfldun.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gppetecqr.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/grdxkderd.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gihdqqxhc.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gpclsnlii.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/glmvgkmmo.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gzbuznodg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gjdgtmldb.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gcotmdamg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/geffspriq.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gdqyeiqya.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gvpjtadpm.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gnikfuyjk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/ggspbtrpa.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/ghlaahueu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gqqbaujdj.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/grnxzpvuc.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/gsztkwfbk.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gvzlqlcjx.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gjmwolysf.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/ggqjwkqfl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/ggsarsjzi.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gwbzolqzk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gjazplbsl.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gibtqeksh.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gozibzysg.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gzuhpaypt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gdadwnybg.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gclbxaxiq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gyvhcxmhk.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gckdmrtkz.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gqffxhznx.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gludpzzpl.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gzkwfxzea.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gifltjdyw.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/giiiwtvfr.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gffyymkjy.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gxwdmoywd.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gveepqipo.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gwockrlwb.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gasdoatvg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gppqgfteu.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gxajglczm.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gdukylxjp.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/gyenwagmv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/glxcgwfpr.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gwkhmfniz.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/gugolgrjf.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gdrjxzuda.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gsttevdsg.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/guwdtjcjm.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gonyfxrus.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/ghclllvis.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gjpkvatej.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gqhnxzdeo.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gemcbdlse.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/ghfqlprhl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gbpktpurk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/gnrsbzufk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gkmpitnni.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gwbctfbrv.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gwoxiobxt.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gwdnuvfpz.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gedzniahh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gxtczafak.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/glxfrjmqn.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/gusconpsv.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/gspjfmfsk.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/ghagnjgse.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gstjbkyii.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gvsyellwx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gzptvzfmg.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gpzuioaob.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gakbygbgc.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gkjssldpd.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fehbvm.com/Article/details/gqmyqpdgk.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gcicsorui.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gyhedkuif.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gbtgjtahy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gctyrnrxa.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gcuhaftyt.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gfxkoxiku.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gpsgtebks.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gwzyhplni.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gwwjirwav.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gjvwhhzte.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gsettflyz.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqwgbmisy.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gnaiuxdvm.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gmnijsljn.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gssxvrdro.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gjinrpfyx.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gyioihmom.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gbcraaaal.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gqpdrpmhf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gsdcyhubw.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gziaqmewl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gifsdbmmq.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gljqxpfrk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gmfhrumpk.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gkaebxbdw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gvrxzesuj.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gfwcccjbx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gynqmrulh.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gyewrckru.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gajnyihsb.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gdcgcxftc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/grzuyeiff.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gyvtdrklo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/givimhkgk.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gabdmracs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gyfiofvaz.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gcuqyonio.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/gltrqyedk.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/grbkqdiwb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gsmqzagyb.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/ghnwjqdar.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gmslofzar.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gtemdmzix.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/grmbgirdk.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gnzrmnurv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gzdkhjaxs.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gjmjiwkmz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/ggptbpiie.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gwuakrfza.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gkcevugpy.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gnaeajxoq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gfzfspoau.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gekxedqah.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/grzyybwnv.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gwzhlwedz.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/ghwrextsd.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gwihbidqz.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/glawuojvd.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gtkecowtq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gpvofzslt.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gpkuencvy.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gxsptvvcs.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gzrlisdvx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/ggykqrewk.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gvbucdagh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gfynnflct.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/glesygggz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gvkcybksk.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gnmltsogw.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gsfqzujsm.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gbovqnabc.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gifkyhhdc.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gvznueuqe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.zdbjq.cn/Article/details/gegpxmmno.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gruwzwctk.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/ggeremnnj.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/glsdytwag.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gicdprmgy.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gdftghook.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gfsynnnfr.sHtML


<!-- 参考信息 -->