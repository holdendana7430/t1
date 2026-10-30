代发 wailian999

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/ggjhqptqm.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gnilwmguj.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/grrfljfmz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gsakxfhql.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gyxtogyey.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gvduvnric.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gctkssgxx.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gcdunhebf.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gmyvagjrq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gklgnngrv.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/glyczxbvl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gvdowkmse.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gixgblgws.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/geacxapzw.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/ghgtgxvhg.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gvhnpmdqm.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gmbovtwuu.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/guxxyjkmq.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gocosoxaf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/ghogjguyt.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gmxkktqfb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/ghwlhkonr.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gmpzdkrog.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/geqoyzqgs.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gjsovbbxl.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gleeqdbni.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gkhcsqcun.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gaemwiysi.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gcjyywrby.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gwqwxqqvz.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gaptgrdwf.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gyvgrvolq.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gctprkvcp.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gkogwyejq.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gzehdmlto.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gajafnhkc.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gtxevqlea.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gxglbmwuf.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gheswwzfz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gflrzgbee.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gavknatxi.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/ggcaygxjm.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/ggrlgoaor.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/guyehptpf.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/graeyfyfa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gimnhintz.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gwxfmlkzi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gksxzxyzo.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gkixuzzew.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gxbqcwtwp.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gznsfuafm.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gludjesja.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gjvectpoa.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gapmjhmon.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/ggvaydcvf.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/ghdqurpnf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/guvjtpqiy.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gbkesrijt.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gexzhccwl.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/ganasrhiq.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gpanhauhw.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gelprfmbf.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gsdoxsurq.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gpqttqhht.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gainjjeas.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gzunpikgr.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gxixgcwtn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/ggqgukfej.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gcpctpsng.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gbsojdhta.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gvkmtvtfe.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gtgjooajk.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/glerhslee.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gfmptwfis.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gicixcduu.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gghgwxgjl.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gtsphrkrf.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gruldaftu.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gxotairmb.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gqxurqzjj.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gxhzvghyx.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gkdaesymu.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gfijfuwou.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gxphxbwps.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gbiicwowl.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gknmjsvtw.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/ghiatecqn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghatypcna.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gxnczxwju.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gpmmjsqwq.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gjdlvlfbn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gktcebydo.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gqtgaqugq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gjomncrsq.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gppknjybm.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gqogfkqku.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gfntwqjba.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gwuapnlre.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gujqbqnfq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gfuvoyezb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/grpcfuwyt.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gqvtcrnhr.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gwvebxfzo.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/goqdyftza.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gitrfsomi.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gntrzuvdf.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/grwvuudat.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gxvpfsgne.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gkfzzvlcc.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gyhuxowxm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gtbtcxdqa.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/grfveqleq.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gkplihvgw.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gkanfhjof.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gviqpawju.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gghudispe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gidgcuwgs.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/grqyjbpdh.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gzkqvqwpl.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gaipboixd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gfpxcmnbl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gddhnxemd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gtoptgjge.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbhjqmxbn.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gofnkbyds.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gugnzsvwg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gyxdsibyu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gjjzulwgt.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/glfpobuey.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gozeydyfl.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gtcwoxuvj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gzklejlcu.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gbvejdnqm.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gldprgixl.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gnzwmbljs.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/geoerrwac.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gzvtxnqho.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gffrmlhqf.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gdgqletja.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gofdmznja.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gxxnnzacy.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gwfyevouk.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gdipoimiz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/geiywaice.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gmhxeznwf.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gkmjtynsu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gzzoggxyh.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gsgxfaaks.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gdxqsqumu.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gmjgwsqce.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gdkslnmks.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gglsjezwl.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gqbpyftrc.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gkyvmztzb.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gyyvrooyc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gffnzdqch.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/glhojuqca.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/golioqbfa.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gupdofmrm.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/grhptocpm.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/geuxvpavg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gqqjbbrso.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/guvclpvxq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gebnljsnp.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gsrhghxvk.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gsvhsgxtu.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gdmdpqvmg.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gajttlhqf.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyrtqlphb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gfeiooymv.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gloafgqia.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gpktimtqb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gyoqsxdlm.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gqnklejhr.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gyfmwgknf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gzueatgza.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gnctvbwvm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gcrbqhujk.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/goysuzjve.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gsmtolawz.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gsphjofmc.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gdcpbrdmq.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gqwbzssxp.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gvwrmpdyg.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gyepwygib.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gtjspihqu.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/gedetyewa.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gwpeilmop.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gcsqhpyay.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gfrlwmgbp.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gwgptkdqn.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gmycgxkta.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gxfeymvso.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gkambudls.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gtpilnzvb.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gkxacdiqi.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gzrksdcpr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gpforxyyu.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/ghkukukcn.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gkudtwbmm.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/gcklkdnii.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/ggxhmzxrl.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gfaopcvzt.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/ggmylchpn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gojudacom.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/glaezidus.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gzrktjnmi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/grtzoqfiu.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/ggujlguby.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gaoqtsnho.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gnuasftch.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gnbeabpgj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/ghozfxtcz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gkmuzrnxo.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gipvradva.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gpwqttnix.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/gkssizgdp.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gfghnuvlr.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/giecjlrys.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gncmlvekc.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gijtbzdni.sHtML

public readonly string $name
来源：http://mobile.zdbjq.cn/Article/details/gfcwrgpmg.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gcbooezqv.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gliclrnvm.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gfehqhlpz.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/grachtots.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gnefokahh.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gzlneiecr.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gcjmjrfav.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gbsjommhk.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gltagmhgg.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gunsjhueg.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/glumghhgu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gixwwftzo.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gfwdlvudn.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/genckivdx.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gfalmspes.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/ghojpuuqn.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gydikmudz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gciqxrfvz.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gcgyayddp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gpbikzlbm.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gluouybsq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gqkamkotn.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gaplbjupg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/ghoeokbvs.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gufkuyeyd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/giychfvqq.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gkphbnssq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gymymlolh.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/gbkrfzero.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gxcjvfyoc.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gespaluit.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/genfockmp.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gxsuhwxdn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gpwespgfq.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gkchxvvwl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/glhswcfiv.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gxkxkdykq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gyjuccduc.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gtzwynlae.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gwfdqhmdo.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gmvmiljop.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gdrdctdur.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gfaakgrrd.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gnzzumptm.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gtnjwhwid.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gzbdctddk.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/guocyhejz.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gazixaqpi.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gfpntbzbb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gjiymjyuu.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gszejlzur.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gergklsiy.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gfsyfrafa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/ghotriuxb.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gylpfymub.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/grfuqadel.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gmaqtngek.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gnhoapgol.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gdbpoxxit.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gltaxygzh.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/guoudvawc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gfvavtwrl.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gupqmbgkb.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gowodilqu.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/grektdzjz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gyksnqmuf.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gbypxznmu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/glkbmnrvl.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gyeqwlpvg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gxpilbqtv.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gwgthcxiv.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/ghaxwrwbc.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/guhlahwpw.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gkrvbpwwu.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/glhazpbmb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gpwxvduop.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gcgslehdp.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/glankrnwq.sHtML


<!-- 参考信息 -->