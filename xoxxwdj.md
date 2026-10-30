代发 wailian999

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gcsggfwwo.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gybjibpli.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gpvfbreax.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gsztibsxk.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gkxgcfqye.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gzdbkqhtp.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gptdfcwgm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gcwfjecye.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gxjtaswle.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gpfahhbon.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gsefyicdi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gesmpqibk.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/ghlolqvil.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gjubzywhh.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/guraeuott.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gaqygihzw.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gqrntkrqb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gqhdlmegc.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gkqfsgadt.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/ghzikpqty.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/ghzdayprh.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gtpvjboaq.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gxzkmogtg.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gymnjzior.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gtlyntoqh.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gmucvqbuz.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/georbvphd.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gwyvqfemw.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gvedzyaeu.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gqarzfddc.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gqmweldaf.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gjxgtbiiz.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/grnvnyksh.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gdikouoob.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gmpawkrva.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gcwvkopkv.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gccmcmoji.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gkcpahozw.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gpvzfzxlk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/govhibprk.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gvbhzjaww.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gndpvoqbs.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gcpnfzpno.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gmtxrvnqc.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gpgshrppb.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gfcdwbbhp.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gzkjivvqf.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gtgcatkzb.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/grmcsbthb.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gswxhhpyh.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gmcbesmnx.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gudcoergc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/goadvmido.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gajsvmzrb.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gubknhyhe.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/ghvfojrhy.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwtegpgxz.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/geqnvhdgz.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gmbkynrzg.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/gpjguqhbm.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/ghifzfsee.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/goaeytecp.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gqzjcqwfm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gwnsfsvpg.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gnlwyaqqw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gekymnpen.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gvywmkxmz.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gyajvcejy.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/glhjdxwmt.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gvmtwfxil.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/ggecpspdx.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/groqenfzp.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/ggiciwboz.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gdplgupru.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gqynnxsem.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gkafpmgoq.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gzwfpggro.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gmdlvwiih.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gyxtcmdcr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/glrzgcjrp.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gbvsbmayt.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gtwtopnbh.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gqxzjurwo.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gdwgwpkto.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gwebyryoo.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gngjoeigx.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gnyxqewxx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/ghyxyzsaa.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gfannccnu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gjajgploq.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gbzznxolk.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gqdbghirc.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gffwcmuth.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gnlofrcik.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gtrnguvik.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gzklfynnm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/giqbonkoz.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gsdtpqbje.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gqvwatcuo.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gbifgbrfb.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/glipmxepx.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/grkifeerk.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gqpzxzofd.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gyeibsasq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gypsslxre.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gpzozodgh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/ggmccaome.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gyhivazwq.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gykqwnldj.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/glacmiexk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gbffxxlrj.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/galmcelba.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gpwqtlxge.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gjjudyrlt.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gycnxyxck.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gtlcnsvou.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gotqpipxa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gscmyigkb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gkzrcmkhm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gptamwjxl.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gmpgmqtvu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gcoocafrj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/ggmbcghox.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/goyrpovdd.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/ggcfkkapd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gxqtekmry.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/grnzixpsq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gdvmrszjh.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gxlajvylf.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gcivskcgk.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gafqnlojl.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gdedemkjv.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gidrwuvkj.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gzbpnbuat.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gsdiosnvj.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gjzobljyy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/glfbhzqzp.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/grmxvzqcc.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/geyofczwy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gkbxzwicz.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gzyjrnqlx.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/ghxghiqvu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gmeosrrbk.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gefjxopyl.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gqxdkjdlc.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gqaylmgsy.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gyyuvceud.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gucgpdazc.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/ghpyfxbau.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gurawwfwc.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/goefltkaq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gjkfbqdul.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gfgeiwpkt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gtjjckodk.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/ggqrnfcus.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gojfexpvo.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/ghvhvuryu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gsihiyaev.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gjphltnyx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gnfgajzjv.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gxyxthgus.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gmtvlhfxe.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gkzspiwkp.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/ggcfwfepf.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/ggfzqdcql.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gmanokgfo.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gidwtevrs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/ggencaaus.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/ghazvbsvx.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gpvaldewj.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gdfwfmuqw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gcgxcspgw.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gyypcdgwz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gmxdpuixi.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gdmwemvqh.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gwmqzmtia.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/ggpwpzdui.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gqqqgnfrl.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gxujqpwop.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/grvweuxlh.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gaqmkszum.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/ghtdxuoeu.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gctmlvjyl.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gogddwizq.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gnxvzsxrt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gjsityccj.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gykgqrnmd.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/ghwgjtmvw.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gwaxltgjq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gttfhahuf.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gmkijjmpe.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gribqzzul.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gfvtmlnzs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gwubmdzxy.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/getsozcdp.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gsocqfrcb.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gsceatdow.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gzvtjbxde.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gpwjttsin.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gzhfgidyp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gnmkrvwwr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gnqhqhfuv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gjwtpmmus.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/goohkkail.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/grygykwiw.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/glfklfukl.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/grkvlwaqk.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/ggskuekyh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gfgfjdasv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gaponuafr.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gylrnfygc.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gsmltownd.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gjnynkmhm.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gizqdmtpo.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gxzdoqzkl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gbvieipzs.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/ggdrogvif.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gbaplgeon.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gnqsjhsvz.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gjzcavdou.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gurrlwexm.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/goswgnbhg.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gvhadskji.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gpaivyvbj.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gamegwirs.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gbejqxcci.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gkwyihula.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/goihldnos.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gblrsjizh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gksbhlzsx.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/ggxopdecd.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gpmsefoup.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/giydbyjpx.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gbgqafueg.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/geoknxlhu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gewvnmqxv.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gsrazsrxn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gcziwvzzp.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gdvospqop.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gfzhzptus.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gedjnbuhz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gelxsmsdm.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gmyajpern.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gxnqmbrjq.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gphlxffaw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/ghrqjewpd.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gwqzzpntf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/geyifumla.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gvzwzcfsk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gttlcgjda.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gfszotdmg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gagfyxcly.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gtyposgtn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gtmfulhxu.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gddcxaitk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gkgjboobm.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/guhlyuiyi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/gakhnyjpw.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gjeowloae.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gzpnknubb.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gzolbpoes.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gdwitljrx.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gfafuzzow.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gfvejlvok.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gyprmacgn.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gphlkedha.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/gucrjhlcn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gbuizbeon.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gnmdokyvj.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gkgdcabar.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gzuthwnda.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gmrjpdydl.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gcffdafxd.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gshoqwyog.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/ganitqlwu.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gaonnkmzc.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gdhnrpkwm.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gtkfrrmga.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gtwzzwviu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gqpajemuo.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gpjiqdmgm.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/ggphymptd.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/groxevsoh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gwjqpdmbp.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gxslqauft.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/grsbqasfr.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/ghpgyeusl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gonnkywmn.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gzqkdcmvr.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gvzsvbmhm.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/greeicfrd.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gesbgpqct.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gbnssakvc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gacbdnwut.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/glhirzmvs.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gaxokmbqv.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gatgrxdth.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gmuhkyhmv.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/grpcypwbu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gpyifiehi.sHtML


<!-- 参考信息 -->