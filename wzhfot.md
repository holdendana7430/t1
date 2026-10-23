代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3twzogihe.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pcbcufkw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3jescahjs.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3sdmykfwg.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3eftensie.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3qmjhhukk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ivwnjris.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lrwrdvif.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bihghgiw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3tzolssaz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3kkncuofg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3msxtmlpt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3pzwmtsuh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3cujvcyoq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3tcdugygu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3yvikipga.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3qwrdbldu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3vvsnlnnb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vqyggqxz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xfnwidkm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wucpckup.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eqgemkwz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ttszxwjd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qimkxjwa.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3zqwkeocg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3cuqwxpio.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rkdwtyzj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nmalytme.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3lakwzblt.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3tqcwajgq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3abtfaotr.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3dmjzaqim.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3mdfxpgsr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3cqgsxdpd.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3hsfpltly.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3llubylcq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jnhrwxfm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3lszdtlsi.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3xcvhfofd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lzcprdqu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3raaccphl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3lefknhpf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3fhmuxads.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ugtcjgxe.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3mhaxezug.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ynxqfsso.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3sbywjlbh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3jlzlzbeq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3cmadllgt.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3xdjzslvw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ttaycpbr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3tpvjmprh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3zgtzhlyi.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3elopnghv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3avwlpynm.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3tryhxdhd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ocvtjucf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tlqfvmio.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3lpogkapm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3fvfyryyz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3qhhnhwda.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3dvmtrafw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ounbpaep.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3chqqdbug.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3mqtakbdl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xlivbtxh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3yyzezvrt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zokkjvud.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3utubdgmw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3imqowwcs.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xsxarnxn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3xbnnzeuo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jbmrowek.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3oxeudzmb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3jitnutiz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3twcyvnxd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vdblmcqx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3iyjxaccr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ekoegpec.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3khjwodak.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ahunacmr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xdvvqoxn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qfahaoip.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcvmwmod.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3elamlflv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwogcivm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3qrqojixh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xchaoyvf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3aynwnrxx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlgkrrfk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xgluvali.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3xzrmcvpb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ugbpfxkw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jvvhvokd.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ojlpetzt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3tdhrbpna.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3gzliwwkz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aiuskhte.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bhotnbmv.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3dqouftbo.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ylaoxsmj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xnkimxya.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3sdmtuuot.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ezttppln.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iliwzsug.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mmghttpt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3mxdaskbv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3njjcmjyx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3dqivwwcq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xeabedvn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qxtmjowa.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3fddyuudo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3elajfage.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3oltfwhqi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3izcfigrd.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3artdrceg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3afkhguei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yrdfilrh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xjxttols.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swmofzgw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3smgtkamz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3cgdcclmr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3kffbrnil.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fozgbvpi.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3spnsbhks.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3nazzhlvl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ueyugnxd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ipwfabrj.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3dlkjazpo.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qzkioqhw.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ypbxfkiq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ggfyswoy.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3dafydnae.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3oiueyyhg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3urseeczz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3guniunci.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3itwdmtwt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3qyebhcjp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3kugunuks.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3pwlkkpxk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jweoccyo.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3agbghkyd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3brdyvzwo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hurgmpfz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3xigbvdwm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3hbuirzif.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3vuemurzu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fcjpwppk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3sumyljzc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3pdjxjkdt.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3acifkzpz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3tnczgwer.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3apilydjy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3hafvyzqw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3zfdupjqh.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dbcvgoem.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rwiyipcs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3tviopeug.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ihmeuicu.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3paazpkhl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3bjsodlqt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3omadhrqq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ooxchnbp.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3uhtcfylc.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3avayxvda.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3epjjodoc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3swlbhjjt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wrlkewsl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3buutnyak.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ohyozhyl.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3iiniumin.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ojlyrlkk.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3axtzohsp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3qpwcgjbr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3usiovzrv.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3fkmvikzv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3hgauleso.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3rtlppirg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3kxbjvvbm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3seibnrpt.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3oktqwncb.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3pxixriky.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3pvhsghgs.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3oamrzxic.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3nqwriekp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3jgbwvnes.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3uamabyei.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qgfceixd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3zzvlpycp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3kvqyjpmj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3yyobywif.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3tkvcyfvj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3gshzliyo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3nmmthcee.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3aqqbgerj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3wemywfda.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3btzrttfn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3rnmlffcn.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3jvfnnkhu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3pewwbppd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3qgasgefo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3aldhxidi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ewfdydnh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3secshcle.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3uspxraxj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3pqwcqyjl.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3uemzudhd.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3tpqfjond.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3vfyzjfzx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nkvmegrt.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3mdeptndo.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3nhfpvjbz.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3wafawppq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3feozfgsl.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3tesxuhkt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvokudyq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3clyotcyo.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3yltnrwww.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3bugdeckb.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcmfcqrz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3efvzxuyx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ildcdpeg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xkwfzoge.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3uwqlligd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3jgtzibdv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ljmgenji.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3rlwkzbbk.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3upmrxjym.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3skwgvjqx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fjwrgxdu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3paujhdji.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3udiktpll.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3elynukwv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ndaotlbs.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3fjpjjoha.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pupmwbkq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3bzrkqcry.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nvaluwvg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3hxndxvmo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lymizvtd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3dyvikohz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3cdykzzjk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3uhjxwfmj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3cyblgsrw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3xbgdsrtx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3eqdugxow.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gtohsnpl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3rcsrzxsz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3chghgzqx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tunghatf.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3rzyurfos.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3knuorusq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3bdejmcso.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3fokrzeex.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ykrgkoti.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3lrvpgmcs.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3peomrfxh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3tueaelzf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3vuehxjwg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3zvuwtnkr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3eiicjypu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3otwivvgy.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3muqdhlde.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3xumuijnj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3llhzjdpp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ncbsmfix.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ifhxoaoh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3cywoaudn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3qvxsqvqh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3vsueoufu.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3zjuhfacn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3pukxjtge.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3rcbpnoiy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3jrehnhfd.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3gmngqtee.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3kxwtaoro.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3oqkvnbat.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3terzsmlu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vgizmzjs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3osaqkcmi.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3fantozsw.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3jttyxnkh.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3bgdtxpkv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3hbcoozky.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3fzqhhktg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3oqcxejfp.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3sxruxcap.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3vprssskq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3vkipuohs.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3pteoxmol.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3sbbmjkwk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3iauxkkdz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3oszccsvc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3vozrqhqa.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3sfqrbgdb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3nmaemady.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3wtvddfjy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cunjbfdj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3xvkmgbou.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gykpszeo.html


<!-- 参考信息 -->