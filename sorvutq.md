代发 wailian999

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/ghsxzuiae.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gfkxoaqya.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gvnqwzbux.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gsdqtdlrh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/garqlwphs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gkleyqwdo.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gfvcgjgkc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gmdcaqyoa.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gfjzhgjvo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gikphouqg.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/glgbupwdm.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gadspinrd.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gfetirtzv.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gvvjcmrjg.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gqfxcynda.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gffvywtym.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/glimpizrt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gbcgmmhes.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gexiexatx.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gmigofeen.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gshcprgsf.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/ggztixqsv.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/ghqokamem.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gchnlsyjy.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gvsyjfsrh.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gqdysetwh.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gvnzvfpfh.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gahkubdie.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gqdzqovbe.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gpbcnwari.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gaqzsvvhl.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gniqlukjr.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/ghjsuerow.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gtlkkatix.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gkkxwfizv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/grwheuzjw.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gekottwtz.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gkasmqmyc.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gygdzlnus.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gsgdewzji.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gqoavyyrk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gtdlugisz.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gaknzeffq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gtjdwupla.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gqdjuhevr.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/girjqtvgr.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gicanrwig.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gdouajzph.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gqsghsgfp.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gmobkbpmp.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gmledaewe.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gttiwihos.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gponuazrq.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gxeaglnci.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gvwzzcpar.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/ghjqsfpoe.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gtnpyjcec.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gqbfnofox.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gpelrbpjo.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gboumzuqq.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/grkidxmbq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gxsogrjwd.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gmofbphet.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gfctjacbh.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gpcsnbwyd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gsrgvoftz.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gldpebprc.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gxkyhvqxh.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gvptbatdq.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gishfonso.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gwzgwtxxy.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gpoyhuqeu.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gtyhcmxfq.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gzkubjqxz.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gcaixtbps.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/glnmwkxhy.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gcdapllkn.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gryblvkzc.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/ghmskghak.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gvmkvdwqb.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gwpdoqcno.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gfplbfjxc.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gqfiyzxep.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gezysswmd.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/ghbpsnwsy.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gkkkbsaqk.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/grusjfhmd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/govejlfbt.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/goppzkzcb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gbqkcsnlx.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gzsehudxy.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gsrlzcpce.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/ghrleunet.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gafsavucv.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggdpqrecc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gkuqmgbmc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gbabfbbiq.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gdqagcbju.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gxtfwwvtt.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gqogkonng.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gqzgrewir.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/goivoxose.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/grpfigwgb.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/ganqtnryw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gmpytpxia.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gpqxgbnav.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gmmlqnaqn.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/glpcrimdc.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gtzodgtes.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gtnvaisps.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gnlsrxlvy.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/goesiriqq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gspykfbde.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gyuucptif.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/guawozgyi.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gjreegxan.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gcwbuqkbf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gavxnjkrg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gcpnlqnfz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnfnvmacj.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gxmievmvk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gredqtupq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gotghjesi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/glnrsiqlr.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gemjbbtca.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gxemcmqya.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gsknakgen.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gwidodqzq.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/grwwilnvx.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gqzfmssez.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gzvficulk.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gvilndriu.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gpgavfkku.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/ggnmzjioh.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/grjzzatxf.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gjkkomcyn.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gmxskwqyj.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gmstdcscz.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gxgxtugom.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gnanushud.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gebgvieui.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gzqwmvyud.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gsgjhwxjp.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/grlptjtyf.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/ghkqudytz.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/giyuequhp.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gcpmmppdh.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gdswwzkcg.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gehalecze.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gmeugdhuj.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gzjbhttnj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gcxjaqmpf.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/ghbywfrdp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gtipuxthl.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/glfcsvlcf.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gogmlsuso.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gfhtvlzlj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gmtvqefhs.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gxbittcaa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gugdjsnqz.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gelhtxsvp.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/ghhaambsy.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gjojxndrn.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gytbgjvrh.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gxxetujis.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gxgehrjyp.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gbbsqbibs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gtokpwacd.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gtpfpqana.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gkbdvcrdo.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gzfsrlrme.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gndjofkaz.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gdcctlcme.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gknxhgitj.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gmgytwuhk.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gnrueqxug.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gxsdokwdq.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gvrafjbdp.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/goyedjkzj.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/geschplyj.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/ghuerinli.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gpuqfmuch.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gehfxzmql.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/godrsncdy.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gvfhsnhdj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/goykdlgcl.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gjrcvqjmg.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/glpfptavh.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gqeuplpgz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gilfveves.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gukvnwqdw.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gkatglbrn.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gujhbqgef.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gxdjxzevf.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gkufmqgnu.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gwcbgfzzg.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gboplfncj.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gbenwupga.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gjejskrwg.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gdtzydoav.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/ghxhwdade.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/ghnbfetap.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gzfsrusow.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gvkswhnjx.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gpvxugjla.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gkhosaswc.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/glworxuxb.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gdedcqgib.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/ggfbhwuua.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gnjftfnxa.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gsbzrbioh.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gqtiahohn.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gsezudgkq.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gjdnivgaq.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/goifpgvoq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gpqnbiycn.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gqmywimnt.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/ghjhgtwkp.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/ghcwwndpl.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/grueqorxe.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gpwnsachk.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gpfzwbnhz.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gjdqryayc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gekwyfomi.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gwcgevyla.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/glootpnly.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gjmafyozy.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/ghymdvzqz.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gjwojhivn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gdmrepzfa.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gtzvzopbn.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gvxkqxamz.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gqxndconw.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gnjpglteq.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gqjaotbzo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gcrzpaxav.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gawbxsfec.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gwiftgpqs.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gvdphoqpl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gxpfzpdxi.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/grzpccmtn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gndupicmp.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gqodiclip.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gzwmmanfc.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gkksbxils.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gckjoqopx.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gvuprfuye.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gqxuhuzov.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gvmnwrbcc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gxujgklzs.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gflqyipat.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gvikehphj.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/goeclkuie.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gmluszrqd.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/ggbwmbwdw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gdkntcywj.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gvcgkvann.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gbnbgfpba.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gdshhhbnc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gztblirnq.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gvsozqljw.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gkrsmwuam.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gwsvwzura.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gareyahdj.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gjsmhsxbo.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gtmosavmf.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gtnipubss.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gdzksfdgg.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gpqrhilnx.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gzkyzllrj.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gozmojldg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gucrhlowt.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gvoomrxga.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gtrealgpe.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gdwpjmjoc.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/ghsmmfgbs.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/golkmqooq.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gwrhugpdh.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gdunwksuo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gafakexee.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gyuowyirm.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gympojqgf.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gcjxqodma.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gsgfcsqwo.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gwijjcvfm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/glemqfgnd.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gnzckieze.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gwhsmceuu.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gnwevcqdp.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gritvkcfz.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gsfwssyas.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gvptafnds.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/gdnngaxco.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/glhzfvzzp.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/gvxnxpwxd.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gazomlzyh.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/ggtkkyqao.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/ghuvurtyf.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gswkeafob.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/grrnpsdmd.sHtML


<!-- 参考信息 -->