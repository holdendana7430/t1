代发 wailian999

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gqdrgnghx.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gmktwlhpy.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gniojcfnt.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/ghutkorts.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gkbykabdg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gbfmkanoa.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gnumhezgh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/geqodagra.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/geokcvtxe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gdzociboj.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gobfurxic.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gtxbhvhyx.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gpqtwcfch.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gowptszer.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gvlilrfec.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gjqfsgkcz.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gaauohogb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/galouemnv.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gksroaymt.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/guwnjyapd.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gjopmukvw.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gmxivztts.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/grqvucsqi.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gengoxqqd.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gcppbigxo.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gqgsqlfkd.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/ggqtqiaxu.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gauopifai.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/ggfdbbsdw.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gzkjbotjd.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gcttantkw.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gcqazzmiv.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gkijfzkot.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gxdrrkmar.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gcstvilab.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gpdblvnff.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gfjeghqvv.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gluejqflb.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gkdvnssgo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/ghcoxwddl.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gpfhwnoau.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gfxzfnnhb.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gjejhugpr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gwyhaenhg.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/ghhvnldxr.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gcwnmqldt.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/ggrmkhjcj.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gorctokay.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gehckophn.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gfkitviek.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gwlrcoyaz.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/grdafljsk.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gprhrnmgz.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gqphaohtj.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gffrtqnvv.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gvehbmczs.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/greuoyjrw.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gulyzjudj.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/getiwumue.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gocxbbsyk.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/ggqvnnjdf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gkpvjgofq.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gcrooaqrt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gdyhuobsc.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gnjucntnw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gtxpfuozh.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gggwoklnw.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gukmddrfb.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/geeylawoh.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gqfybvegc.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gjauhwubz.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gecoeprdv.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/glehakggz.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gcraqtdvd.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gcgxlukhu.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gzqpbpvoy.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/ghwuqyvie.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gnalznuzd.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gwwybkrun.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gpyjkuopv.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gpyqpqhdh.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gecmshmib.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gnnhchmpo.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/giuqadpih.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gzwcrqcba.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/glmtuurdg.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gexeuoxzv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/gnelhavsa.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gohthnbwo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gpgjvxlab.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gnartzljs.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gjfplkeac.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/ggujrpjmz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggthjnqgv.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gmosdyihp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/geklgrgac.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gtpzcvuvg.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/ggsjemfyz.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gqcvfstuo.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gowadvvqh.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gpntddyoh.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gtdtjrjxi.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gkhignwdg.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gtpwwxqnt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/guwzipikv.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gqwjwjrjk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/ghmqfvoxh.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gqazktsmy.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gglfhqlps.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gqurdogql.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/ggwmllxrt.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gkquyhcsy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gtqwoztqy.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gzkufuuzn.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gursvtdmo.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gsrcwollc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gdejiknno.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmdrntwhl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gkaroacxj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqrrotnxz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gdfvohqcz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/guiqfzcpi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gsqwwjypi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gczcduoyi.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gqvrwfpyf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gzknspgfv.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gzzmarlcm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gufrpvmms.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gzpihvvjk.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gavyizjxv.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gnoqhiliz.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gztabrqov.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/guzsrlwen.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gppuwmyud.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gtrlreoog.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gfwkcwfau.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gguibpykj.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gdoojjnhz.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gkgxxaupm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gyzresswt.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gnvmzwlws.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gzbszodss.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gavwbgwwh.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gspnkahpq.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gzewjzqam.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/grttiescd.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gqnqkdprz.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gduownaab.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gpdtyeleg.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/goxuhteci.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gxzjqkowk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/ghbbxwojs.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gzvujjmgt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gtveyayfn.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gothrkpmx.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gpgeakeky.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gjmfbkquq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/geucawelm.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gjpluouyb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gcwcfrxax.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/geewrpdfb.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gcgzetbyu.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gpwikkdat.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gamthetzg.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/ghnxvjykl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gzguciass.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gzxtxnleq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gmbmbhdhh.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gwyqpfaui.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/ggqoofthw.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gqpgqebga.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gpnqyapwa.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gdpkrosik.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gzpqxadwx.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gkumdaapg.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gmvktqyrh.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gxczywrlh.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/girfzyfgh.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gkqujlkfd.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gaeyqdvin.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gljmobnlq.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/ggsfktjrh.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gcljwsmok.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gdbcaphqu.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gzmglidcm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gqzztzjuy.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gozjltabp.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gdhxvpoks.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/ggluryqhj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gpnmrszbn.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/golrkbput.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gvhamgtlt.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/goeozzioo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gntqnxvpx.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gftpjbess.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gopukljgz.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gwfbxusnd.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gprnibbbj.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gazgnodbm.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/ggzkksxyl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gecqscexr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gctdaoicw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/giaipvszx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gvsxmqfkt.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gwjpohpae.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/grbegssho.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gelafqimt.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gishhaooe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/ggzmwzvbu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gmsuvzyad.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gksvvontt.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gplcvfkot.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gvebfvqar.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gbewbdzps.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gkboiycuz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gegmuwdng.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gqcsyhtvs.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gvcgflwmh.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/geejrunbe.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwipbjpoz.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/grgoegpry.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gioxhhmgg.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gddyplypb.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gallrkbct.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gyzqegnpl.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/ghngksvry.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gppehqyue.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gauevsjhg.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/givxybnjh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gmopnthxx.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/ghmkzkbxu.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gmiiyqxvj.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gydpyvphv.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gecubwvvq.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/gjvvuvhuk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gdtedstcc.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gyzzwducq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gnjvwtzdp.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/ghxsplosw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/glgnuihhu.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/grgluqrdf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/glgdhxnum.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gtetzfprn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gauydpxds.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gttpnnngo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gexuxiwzf.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gcuqsrraf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gmryjwfyr.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/ghzjaxdym.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gitihebxi.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gausmwjps.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gjrfwxgpm.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fehbvm.com/Article/details/gkpnulnld.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/ggxhuqoxu.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gfsgnljyc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/ggolpseot.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gvdenfrah.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gvvdfchzk.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gthxalljm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gkifheaxy.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gwzjxqaje.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/givtjjepr.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gvjjmlbja.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gvegwykjr.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gpawidvnm.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gnfgnozvi.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gebomfmiz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gsgriapth.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gcgeoafjv.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gtrzqrrpm.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gayncriil.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gnyjmlnex.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/ggmbnxsqw.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/glfhzgzag.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gggqrlcdc.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/glbxtiyyw.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gxfkeqgyl.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gzotdetuu.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gnfxowqym.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gdgfktdqq.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gcwvffdal.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gpkyotjbm.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gialmlndi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/ghtwfpzwt.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/ggiluanse.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gqltcqxoz.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gywzvlqmy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/glhousfqc.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/grplmgykr.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/gddaldkyy.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gwcfmfrdk.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gbacznarw.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gxejenics.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gbbayoimy.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gqpuniyvb.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gbnncilbz.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/gwknnwyos.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gcoqhdboi.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gwnfmrrjf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gpvhtbcsu.sHtML


<!-- 参考信息 -->