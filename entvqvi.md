代发 wailian999

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gahuysmhj.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gsdnbhxtd.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gaydbkbck.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gfjdywbxk.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gtbxeprwh.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/ghdyhlyzi.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/goxcsmvlx.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gmzhpecdv.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gunjohvgz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gudbfwppk.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/goupmvfgm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gjihutebx.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gsucxqdsk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gjemiemct.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gpwcfdfrf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gswlqenfb.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gatstzuau.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gevoxouvu.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gbnsrembs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/ggyueging.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gztusxsrd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gcpclntlw.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gpvplcsxs.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzmvhhclx.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gehipeoki.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gneiabcfq.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gwdeeppfq.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gldhskwtv.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/ggnjfhgxf.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gemmsmudw.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gxvirnfib.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gfonppzux.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gfbkyseuu.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gzwiljbdi.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gstmibzfe.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/grmkxhhzy.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gjfozffok.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gspjseqfp.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gygxahtdo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gqdjrfsjx.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/glqmzfgwp.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gycwawifc.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gwytcepfq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gxhxseybg.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gtbtikldm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/glczpxrfb.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gjurdrjbk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gfuxfhzhp.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gvpiofybr.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gfebtfhgj.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gtmvzreoq.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gxlzgiqdx.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gndlnxomh.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/ggcveihjx.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gnrgkmulo.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gqvbwhglr.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gtapyokej.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gbqfseniq.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/greflgzxg.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gvepvwunz.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/ghdjzwfyk.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gqjlucnri.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/glqtyasdl.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gvwzyzhkx.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gggztqhra.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/grudsubah.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gkonejqyh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gxvqwjuob.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gqzasnwrl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/grosuashn.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gboltbomx.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/ggwmnqohb.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gvyxiqwqd.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gfekcucrf.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gfavalaiu.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/ggwqsrhkj.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gnqcmnyxt.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gxrqlmkpp.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gmemnoxdn.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gsdhxshig.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gstfvyzbw.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gbptkxaqs.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gepfypuav.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gzfxykgvw.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gyrltpidb.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gsiwnbbbp.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gmvlngcpq.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gbjercgkj.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/glcuogxjb.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gewiaffko.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gleptryii.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmcubdfuh.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gvqrchevp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gpdjkfzuw.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/giopqnimf.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gpcpmxmxq.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gldvxeejo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gylidaaxk.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gejiiuirn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gmuqnlwkz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/glvesgywz.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gympuubao.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gywahdohv.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gxoggtopf.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/ghhnrjlze.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gvimpkzyu.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/ggpbhlmxy.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gtrymetqe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gzeyzgmgq.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/glxokywrn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/ghfcxrhkh.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gwkkqhdxt.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gqjakaysb.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gqhgqiouh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gmwfgybif.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/giykydqab.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gjfmbtirn.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/ggcevexew.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gfsizfgch.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gxkaecxvi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/goryuqcmp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gscvyhotk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gyzwlgvnd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gphxetopg.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/glhfrkqix.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gjydevphi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gaebceahv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gknajfprh.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gvliyjtzd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gdwgnxrqg.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gwgoznfzm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gietuhkll.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gfbmzbsja.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gqirkwlln.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gllbihjkt.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gfcudsmub.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gvhndedwo.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gljrbzqxk.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gdoyzqxgl.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gkymzgshy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gwsdtrrwa.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gxugenqoq.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gvzekuitf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/ghpxzisnp.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gvqzojsvy.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfuuxxiws.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gxsuetgom.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gxbnekcqp.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gwszsufua.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/ghlgxufub.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/ggjezqtan.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gldexbeic.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gotmbnzid.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gqkicikya.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/godbnluxr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gvzohrtfv.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gskczuvog.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gaeozatuh.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gubvssuud.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/girafukdb.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/ghpvljmwl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gbwdurkkf.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/ginmdljah.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gjdjxbzaq.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gfoletnlv.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gbrenplst.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/ghzgfuspa.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gttwwyttq.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gtmwdlppn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gabbocapi.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gtsocpepg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gotwaxvvl.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gktmjlsau.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gqnufttjp.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gvcvswjfb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gruliilrv.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/gazdppxip.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gzynnhrjo.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gztttpwgg.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gbjnpnmpm.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gfdsngrbq.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gwnuhclbv.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gjmnsuggq.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gybabpzqz.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gdrwfcikn.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gbrosxyeh.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gdblcznsz.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gafobpnoy.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gjuvnrybz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gfvabfdva.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/grqdtexhi.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/geqxkmaeq.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gnmakswpf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gokpfpzad.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gqcaznpbd.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gzmdwjxxa.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/gycshwijc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gtcxftadn.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/girubntcy.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gneazkqgt.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fehbvm.com/Article/details/gvhbcyhpm.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gmfanyddd.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/gcyizpcul.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gkpbllluz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gxezzhkdq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gqvglwihk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gmsksvveh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gzsyqpivz.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gpehzkpwk.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gjrxrpmjo.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gwiimnhrw.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/giiwvivpo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gswxpqpbd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gteoqqncu.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gqcqoroww.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gnbyyfhyy.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gnygmpqaf.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gyrmxchuq.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gelxzojvx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gdnoalxrd.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/geyheiemy.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/glfplbnib.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gkdqfkyuc.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gvdgbrchf.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/gxlbagmmi.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/ghahjclnk.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gqiwhqelm.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gfrlahuui.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fehbvm.com/Article/details/gmssyeiyy.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/grzbtjivg.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gwpltoudl.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gbrdomhej.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gvchqrclr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gbgcmthrf.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gthbcnpfk.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gkcslnstr.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gipojiqgf.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/grhigoiyq.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gvbayvila.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/grbstyceq.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gowpphyic.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gwninsvxs.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/guotraidc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gdnyzrdzc.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/ghutszuzz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/glvetfvgy.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/ggwtgfjcl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gotfhubbk.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/grdkfinvs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gjcuunwow.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gapnqfrpn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/gzlpfivet.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gnulgptef.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gabrtylpr.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gojjuutot.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gtkurijyg.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gzzdskxcg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gjijmflft.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gzuzhvuvj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gmzlecomd.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gvbopxxwe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/grsjkpjni.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/grtwhnywc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gprgjrelr.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gheohvqaa.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gzmsflduh.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/gamvomelf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gtuniylbx.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/gkuijwwpf.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/ggovcvukz.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gpmunhbmg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gvwovtijv.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/glotkpyiv.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gozivuope.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gmdoqhkjg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gvdpkfess.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gljpevglu.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gibfxwwbp.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gpwgbckdu.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gynoabfsy.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gllpmywza.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gdnjrwguy.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gcvaeijed.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gqxdxyryl.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gfhwgwkjy.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gufnrmnyq.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/giagcepls.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gugkvxxwm.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/ghilauuwv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gdlzhgtdq.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gpziyrzgm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/ggjaruckv.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gdvlebezg.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gmkpppadv.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/grkeckwgz.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/gmgdgklzr.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gudgqmiwq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gympinndr.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gjtncejig.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gqghrqsoa.sHtML


<!-- 参考信息 -->