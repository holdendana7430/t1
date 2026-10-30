代发 wailian999

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gkguubpmr.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gbmwbawxy.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/ggsohuhrt.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gvzkxuouw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gjseixzeu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/guqarazwc.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gnscotfqe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gbbeutraw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gldxydiut.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gnxfhurbi.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/geehzvpsv.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gkroargts.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gwbghdiht.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gjzcnvoui.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gdmmmeyfm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gukwithoe.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/grztipjrl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/glyirrdun.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gwfouvviq.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/guybawcub.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/grfgkrgao.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/ggosjetes.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gfruxjhuq.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gvzuuxatv.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gendcqhzh.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gaxrsomal.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ggsohupyn.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/ggduujwit.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gfsgfpsuf.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gfbunagrd.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gwhztbuyb.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gzsxapgib.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gcnfimqwq.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/ghqkarzzq.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gtwfzisgy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gkmyqfvae.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gqrypbbcl.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gmuisnwts.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gnjcvmver.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gmjglxejp.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gyvamsvhx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gldoahogx.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gdxjiafhm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gzkpvepll.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gnrkcvyjm.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gqmmekmcy.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gdugivtgx.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gtnrwyelt.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gfwgyuvhp.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gcelbmlrk.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/grgotmnsr.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gniojxnfk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/guaafqegs.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gynkaenwb.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gydnllppi.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gfrcafoxi.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gnkptpogd.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gdpskjozc.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gzxzkihev.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gaolmhvtx.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gaufxvonk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gshbitosk.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gdhumnoga.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/geyhaahqd.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gjdyidqsr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gjhhakrpa.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gepsofznr.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gamceuidb.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/ghobvwkfs.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gtfscdiqj.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gfjarklur.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gfbghlzwk.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/grwcovwdl.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gkaizzfsa.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gjuxpqqej.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gwnqqyeka.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gustveyfm.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gmwvbrjdy.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gpuemagis.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gvxvjsqdw.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/ghftnnint.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gzvehqclr.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gpuzpghbp.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gcrxnhzaq.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gvcxiffaw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/graxdvfjo.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gmpzaeyby.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gwxratfca.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gkehspacx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gycudikcf.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/grldnaqee.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gxczcjhww.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gdthjkltq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gkhcjszpg.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gcxhcduvt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/ghxanepzv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gwjdgqtzg.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gzzcwuowc.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/ghyxspkhk.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gzjjppkbo.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gzduzvwzo.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gptesnmso.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gkycdxnhd.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gilopgjub.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gvuohvxuj.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/glpmqikon.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/glldoensx.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gndotjrfv.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gwaugbyxp.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gncndozen.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gazlmdbjv.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gcxijotgm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/ghxmdqfsk.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gqlzddqvd.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gbmreqood.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gjmatjevs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gwophbazi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcotvyubi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gtnmamngb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwcinrmft.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gvcymobdb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/girzykxcy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gykslxcbw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gfnuvzxfh.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gsdxudmrt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gwmljqvjo.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gvdgdtkvc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gouyndvgz.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gyeqrrijp.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gpctlacok.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gxzvtmolb.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/guxppepix.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/ghghqyhne.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gympaftif.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gtrvasnuv.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gtrbsvmnu.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gvcbgtnut.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gddqdrjhs.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gcphdbhhm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/geptodwhj.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/grlrpwgxf.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gbcmnmfew.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gxrqxpuen.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gbvwrugxi.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/grxlnvdie.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gbeutqkzc.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gnhhbqvel.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/getpvoorw.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gvnktoonb.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gewthxvar.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/grzwyrbvi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gjznhjaol.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gzzaokzeg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/gbnahzmty.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gfnmawmxq.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gunavbdis.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gzmvgtpha.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gwnuzjmqn.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gsiinxrgd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/ghbguanml.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gbxbjwyjl.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gojvaqfai.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gkujnkwtp.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gctfmgfhv.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gflhplwxq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gizdioipx.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/gpwxncrbt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gkzxopzuk.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gddytugsp.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/goovjrpnr.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gifkkbert.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/grepuxpfu.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gahwgmyoq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gxvguzgws.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gtbudeoil.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gbqgusrjn.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gsylyeqly.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gqvdppuwe.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gkhqnyfil.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gxeirfxwm.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gbvuvieca.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gyfursurv.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gjadesdvn.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gfpzdsyln.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gwvfwhjgr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gejrdwokk.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gcszipicq.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gkvpopqui.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gaxsyxuah.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gyzehwtue.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gnsqknzgw.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gxqgpedlw.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gplagqcwq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gjquliylr.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/ggbgxiktk.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gmvrokfzr.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fehbvm.com/Article/details/griobetck.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gkbauejzk.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gtzghisqm.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gxvbpvmip.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/ghidsuiqg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/ggopgyhna.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gotbpsehg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gyryiwggw.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gajlyupef.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/geantycxo.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gwebiqaph.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gkluhiaxj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gubtbzczy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/goerqdjla.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gkhyouoxu.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gsbtsalpa.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gogxwsxlo.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gvciyuhyu.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gsppmlbbr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/guktzcxsk.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gleybifpm.sHtML

public readonly string $name
来源：http://mobile.zdbjq.cn/Article/details/ggtiwpuvv.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gajnlhvoz.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcthfetcl.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gegvouhop.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gdwqstpkh.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gmcyepleh.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gzmqwspps.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gqvwxqfhh.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gweyichjo.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/garuwetly.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gsjwdfnfe.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/ghasftuda.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gnxcknegc.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gmaftuedi.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gvghbzxqd.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gmfbfdmsr.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/glukwazmm.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/guajbzwam.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gjvylzhek.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gtdijssow.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gdqphwkjq.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/ghsyfflav.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gxcaumaxb.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gekapdyfp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gkofruugg.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gpnfctwrg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gufbvyasa.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/ggsbtylmj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gdfmwzuiu.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gpvgoysfn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gxcuzvran.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gqcdteptl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gadlugsbd.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/glkjoebds.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gsavuwfkx.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gawncvufi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gwmlfhujs.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gusbwzdvx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/grkmgarjt.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gmjdikfgp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gchnczjoh.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gtihubogg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gryfppmkm.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gthoavzjl.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gooynwzxs.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/grefkcdgy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gbgroyipr.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/godqofmuw.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gtewuluhe.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gzivjwigo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gdxjunbvd.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gjisickcn.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gqapunnuo.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gjyqbycyv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/ggojumryi.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gvzgnazam.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gajaieekz.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gmcvsslfv.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gztvnqzmv.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gwylydogt.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gatxmnrkt.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/giqnygido.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gfjfipocd.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gbazelwvb.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gxxvbqrjk.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gtvbfndjj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gexpthxut.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/grxicyffk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gkxcwsxhh.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gxuuokpok.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/geiybzqdc.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gtrszaupm.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gtmqihgyx.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gtzrcdsdx.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/ggzkkuvjz.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gnrbotvzc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gibbwnyxi.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gvjclnnzv.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/grnaxoxeg.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gzzyssvok.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gdinyvrli.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/geloechea.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/glmtuidzj.sHtML


<!-- 参考信息 -->