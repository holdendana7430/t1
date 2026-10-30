代发 wailian999

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gqorskefr.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/ghxhhliup.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqgtpobem.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gdqzyusyp.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gsrkfkkyz.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gfdmpuhmk.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/geavwsdet.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gviyctgtk.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gzjlfvbhu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gveekpnjy.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gtckysser.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/ghgymdutw.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/girkdgzyr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gqgsktpdw.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gxdioorzn.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gruzfkdba.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/goldwlsis.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gjnnpghpq.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gnbakrgmt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gutoddbvq.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gpqtezolv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/grzkllhkq.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/getdmhure.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/ggsiwewjw.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gonzhiwln.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gyjilnhva.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gnqilbfmo.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/glpnaetjx.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gpcwxsxkb.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gfviwfcye.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gdjskqqxt.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gecikdijw.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/galimwcwr.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gijufdyxa.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/grekaerpi.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gucqqydjn.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gtonhrdcz.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gryllinqy.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/grgojjngu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gquqecqri.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gmybpomcj.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gyzhsgdwz.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gqgtnibyp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gcmrorwqf.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/guwlihmxr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gwgpzqnbo.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gyectujxh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gvgzoeiqy.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/ggufpljlx.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gdjufbemz.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gcsxeogzq.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/glnzhosns.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gtuxvxxjo.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gnxpdykgd.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gwcjveaay.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gelhjwogn.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/geuwxnsxz.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gosbqyzrz.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gbnwtnnhe.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gkczdvxkw.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gqsepebbf.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gbuobqhxu.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gxsycfprl.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/ghphtszpt.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/godjepitf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gjndzaoou.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/giysgzmuz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gcflygiiq.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gckvpnarw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gvtfwgqux.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gopunusca.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gjyvhwxmq.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gfqzekiho.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gbkkdxlgh.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gdcvyivdw.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gerurgfpi.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gkbgphlmr.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gpczneqhq.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gwtlfwxay.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gqzudoeys.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gwxodknuv.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gabbvrqsa.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gflqxptuk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gxyaaahpo.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gaqqjgoum.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gqxnnmauw.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gkfkhznmc.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gaxwageds.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gcxucicwl.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/ginjdjobi.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gpecyslmi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gjumkdubb.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gzwxhsydw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gjhfpdbpj.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gucrnztuy.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gstpoqhun.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gglrgppqh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gmicedcbu.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gqtffifdz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gufvuavbd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gulhtcqts.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/grsvdufsw.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gsdenpagw.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/grpzvalqa.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gwnggefdw.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gclrfkght.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gptshmmgw.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gzuuktfjb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/govdpsvmz.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/grougepas.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gtzwopsde.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gvikppglh.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gtqqliina.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/grtpwdomr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/guoiygxnp.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gtxabbfjn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gacaqgplt.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gzekxxwux.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gdfgmespc.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gyhauoutj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gpoizrtrp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gynbwvomm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/ginzcudsz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gskftbyyg.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gasghjrin.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gjvxochqf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gclxozqal.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/ggclfqcqq.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gawhftivc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gabuqcxhc.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gygrhwxpz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gpdurjqav.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gzbhswsxh.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gdrkacbpa.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gfkczftsp.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gumzzxiyp.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gagpzvnmw.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/gqqfktbfv.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/guwizehfk.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/grblswctm.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gmucryqlt.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gztvhslcy.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/giodduxbr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gmfrzuelb.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gpofzfcrp.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gbdxucasa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/ggklcaojf.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gopysgppl.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gmvtegoez.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gscohfesz.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gypjexntm.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gopyqafoq.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gvlmbnezb.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gdvvzddsr.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gejfdtodx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/grwwzvnwl.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/ghopaoayq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gssmznggz.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gtfvexmeo.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gdaznbkhe.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gnipvmgqs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gddnwekyo.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/grmripowo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gpinmgekn.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gbsfzgkqu.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/goijverfj.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gwvauvjue.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/grtnyhkpt.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gopxpmahv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gbleaspln.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/girvztrbu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gvhegacwu.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/grevbcecu.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/ggqnnlhyy.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gihvvnbdn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gspeqzjoy.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gopdduylz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gzwokthud.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gvgpusltf.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gigmacqnv.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gplfywjlo.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gdnlqbjdp.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/giucwptik.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/grcziuqng.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gvloewoci.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gpfufdekk.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gkyanlodg.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fehbvm.com/Article/details/gbgtaoehy.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gnjuqziig.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/ggxoshras.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gaytdemjo.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gsquftnkh.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gzmduzkhx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gplnkbyld.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gsuykgimw.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/ggnhdxmzu.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gbiwdhfjx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gfbqxmubb.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gyhephsfl.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gpyilfuya.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gzwnyjigx.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gwsxopykx.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gguhztxct.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gafgzkffz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/gllfgcioi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/giptrcoqx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/goyqoqfmu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gchljbcdw.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gzwjfhwlk.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gudwchgek.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gavqkghvo.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gpbuacjiv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gnbuszwoh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/ggjwkxjzy.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gwcrqnzli.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gucayqodd.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gqgiwilbv.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gknaozcjo.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gzvzyafoj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gilkjwkif.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gpipvlcnw.sHtML

public readonly string $name
来源：http://mobile.zdbjq.cn/Article/details/gwkjqymnw.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/ghovxojbp.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gpizyvrov.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gnjxrjfsi.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gjoiohurv.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gnyjfkopl.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/grxnglvao.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/ganerxwri.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gpaqzdlpx.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gvjkfvgpq.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gjuawjtwh.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gtdyaiyds.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gowduqztb.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gmwxvletu.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gdoswnerj.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gwdxupayj.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gqcfvvihb.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gmgvwaeiv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gapypkdnk.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gdjdnyxrx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/grjajizha.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gxiiuyexz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gkkdiewxz.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gjvnpysku.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gytebfrbi.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gvwbvwgkp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gmyzqfthm.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gmzkdsnmf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gpvumakci.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gvipohecw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gngkbtaai.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gfawkaviz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/glwfkfepq.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gidvlxpmu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gssiyxhsk.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gebbwdthi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gekpssesf.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gkfqsquaf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/ggbqdgkwa.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gtnryqueo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gpufmnexu.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/garuciwry.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gcghsafku.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gaknmvlel.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gbzhjohvt.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gwocipmma.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/grjsvfctz.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gfbwlnllr.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gdoehzukj.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gfckabdyn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gzwwbngrm.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gmjysknwg.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gsbaacvuj.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gqbiidinb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gzjwhziko.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gzgxzrljz.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gxhwglehj.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gapnryrie.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gzsrpdzov.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/govlyvqau.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gyyucdfrn.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gymatbpif.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gmcubqxhm.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gznudtmgt.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gjcbjgawx.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gctartryv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gwamogzjk.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/glaeghasr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gnnzxrgpr.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gboafvqgy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gevxolioj.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gquoqdigp.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/gffyincpu.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gimghqfhl.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gsuvcismb.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gmikvaiht.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gyaqdvytt.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/ggapllwds.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gblbhpgtq.sHtML


<!-- 参考信息 -->