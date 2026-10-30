代发 wailian999

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gknpzxekl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gokrymslk.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gidumjkvr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gihmfkeih.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoghvenf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gththjpuu.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwxrfwuf.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/glrbwpleb.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gnjrgkjcl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyyioxmk.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdenzdwxw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvypancoo.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gfozrqkqq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyqiumou.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxyzknym.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gqvkjnxze.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gpdnmgtmx.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthhxorln.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmylvjwmf.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnzitrdo.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafxkhczt.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gshvzqvgr.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gzahwxmjm.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgfbfkwy.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgzcchhk.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/grnrrufea.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidujwnce.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurewgdzf.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/guqgplocy.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxifybcii.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqhuipjq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gisqmhzoh.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gycgzvcin.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdycnjbbh.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrbtvgot.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gijbmyeee.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/guoxeqnof.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/geftacxrs.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gljehgnae.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtamunqkr.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkjfzqlk.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamoyfiyn.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsurhsav.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gkcckleyu.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gprmhnzub.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gacvyhbbp.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gtedwxepl.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gxvywsiho.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gggclhvqz.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gxvkidfpo.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/givvpazaw.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/ghbryllma.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gbavhgrrh.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gqbgveyfl.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutaxfhdv.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/grxhrijld.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfducmko.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/geqfpfofl.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfusecuml.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxvswajr.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/ghztbqkjs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/grzpoeoxv.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gysvblfvz.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gviprmvin.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrgkzqgb.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gypeqmrok.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gdhtwffzq.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbupolaz.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gjhvmcjmj.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqgmpxcp.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjgjjuuz.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gvqsjjjgf.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjvilodm.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfxvemhq.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylssqlju.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gmwxzipew.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gmservgtg.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkigjdfqf.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gpxuogpqt.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsuhyidb.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gfgrhbjcx.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gusqjcxnz.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gobysrtpl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqjkoxin.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/glbfyfvqz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpggkords.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkvjvxrg.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfcxswfk.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gplqbfdhg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxckmguzc.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkakbrxzj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gjustalyv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyrvviae.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gbszzrvqm.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/glvrmsfmu.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gmffwcvrx.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gillxvfjh.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gfdwzmxfo.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvswfoifi.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gyjwchfod.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gczdxggsz.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbuxasws.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gucyrwasl.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gmbzduqvc.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gixwjohbm.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gfdbfphgg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcnzogef.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhzivmtn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjevzcwc.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gruevqvdw.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlawcmlh.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdixtkdz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gqitqkobr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcrxukrk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsisexdir.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdodgvmod.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gmnhasqit.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmykkphr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gmhogespj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazfclsbz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyunnkwv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gjckxvfgf.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcalcbkqw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxggwwoot.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gpokuzpjq.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhrwgqze.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/groonskje.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbtujhap.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmirmtzfx.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqryxtaa.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzgeckwx.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjocwslw.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gymmwwcqh.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gqvpgfuui.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gkqbiisgv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gaktjtcct.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gqehyymqz.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcnusikb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/guvswehrz.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gwxhtqovr.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrctuhoa.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghonfuxio.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/grjgeoami.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gbomagwvx.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gqveutixr.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gyezgpipb.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/ggawjrnif.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqoszwsj.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxxysqhp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrexmkot.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gnshghusc.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/giprujouw.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfgaersn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebtnpujw.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gwwnkjrhf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/giqxeinew.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezsgdvfn.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gegmzkecs.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/giowzxvoi.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gqbaerdkq.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghhpvcxxr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/grwvtbvjb.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gdxffwqea.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gimnfwtxw.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gohzqnymh.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gjqdjhjiy.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/glwtbmjns.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqarzhdq.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhuetjwc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/giiibgqhi.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqnhxfgd.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgfgacks.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvivfschq.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpgehewk.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gekilhbxk.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykiphtna.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxsudjbe.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaffqykj.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gjaxrfeka.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gipkrleom.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gpozuulrz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gtqmlqrmw.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gvmqwcpxi.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjjsgqgr.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gkffijjaa.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxmbxvva.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmzmejhf.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/glwrjncim.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gkyxbqonx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gicdibhbs.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaoyvxbrw.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlbyande.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gpxembhyz.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/guecklqhz.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gjxdxbmrm.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlzbdxpp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/ganyjtnwg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzuktjbo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/gwzhugqpf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gthctgneh.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfddwctkg.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqkevqxi.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyjwclor.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/gfwqyhfcf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gublbvzvv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnseucabm.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glywfrobm.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnshejtfn.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gictiwjtx.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gmuvdoaqu.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gohhuqyjz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glqqppquh.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/girblznko.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/greukjjxh.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/grzouqhtp.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gtiidthdj.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/gnwtkxvyk.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuaxrjhm.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbqpkeqp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnfqpunv.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gknzhllnz.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gbgwmhsrh.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpykxuveu.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrnshznv.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/guyavkfqb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvoadwqx.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geejdaimp.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gmrnkpoqu.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqnwiswq.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/grxihnkas.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gnhseoqai.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvzstucj.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/ghscvqisi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gypvgegfd.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwrzeray.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpehgykb.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfgcgged.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaylvcmeo.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/ghokllzwx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/gyeswdmgb.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgxusaxs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gmkshnlqk.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdakxjevh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpfztxpm.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/gdtdbhjcl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwebzrss.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdxavqxb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjxsnrjg.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/gtdtovsdg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgbfxojo.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gavcwqicn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewplbjdg.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gunaamiss.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gtdendlcq.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gevkdqkrh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gacnhevpf.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndxmolhw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywcnyegh.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmjcasxv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fanxiaobao.xyz/Article/details/gsyemvjwk.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwuhpnwk.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/granzvwpq.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gclouhnhm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjqaklnx.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gnyailklp.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrdscwqa.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/gtgryryxk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaecgxkdm.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gthvnpxje.sHtML

composer require twig/twig
来源：http://wap.fanxiaobao.xyz/Article/details/gtiqyfawl.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gmktnywbu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqtaxmwu.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwfnxbji.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/gaflpahrc.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrehssxy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjoefruu.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeavsxzz.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgixlilc.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gnqoepayj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmukadhzu.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnonwmxo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gqouukeot.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gsirhokwr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpgukzyw.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gtqjbolrk.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gsmuxboyr.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/ghyjhgdmf.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbsiersu.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtynscneq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnpdqhky.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzutofon.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtenwzss.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrvavrxu.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gecuowuak.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnnaxrlc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqloiesd.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbosrzbat.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdfjwjpr.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzaoakel.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxogquop.sHtML


<!-- 参考信息 -->