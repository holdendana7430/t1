代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3bxzsoeby.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3myfiporq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3eblqqgmf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3pdowgtpj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3bbtpgdny.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3mrlculuf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3eylllqsq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rmbvnjbd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3byonhsny.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3teifycsp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yaawtpgs.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ekptrgwb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3vcfghgga.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3cttuvtoy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hnzmrrdn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3fhymizzf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3oduyierl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3nbqnpqpu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ytvsovjr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rzaymjux.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3tzrnzvvb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jtcsbtqv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3whcvoxba.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tljxinzt.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ckuombne.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3dturrvbo.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gswhlcve.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fuepzhza.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ixjwgfgd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ozxqbrdl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qdrbzknl.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3arwmyakh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cdagtlzr.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3psdgwjew.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3qxlwmgxu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ksjcdxsi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3mlhtsiqw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3lqqfuoqc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3lwqenoph.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gcbjeqlh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tkjwmghw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3giegskgr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3junzmtgg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vjauclfc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3scujbnel.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ashefrdz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3fhrbwxuv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3bmwdtazc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3unbrtclx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3khtuvxec.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3dbtmwbst.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3nvvjlleg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zbdjckhf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3yipsavaq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mixojiek.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3yodrkhlf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qsopijzb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hlgnkasi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qktyisnm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dxnluumz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3nxlyrgxv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3eocuqjjz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3kkdgkkte.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3adiknvrl.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3nykzfnec.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3aeccwxnm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ufcjztgk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xvdythsk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3yohravaz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3zufcttrq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3dhfglqno.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3wolgsyjr.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bsecurxu.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mwnnnskl.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3nwhtamhj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ixotnwot.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tmzvaoky.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3hoamtphm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3rnwuzsia.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3meqtwzmh.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lkqvehth.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3lgbndlnc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rgsdtush.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sknukcdp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3kagjvxdk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldibpqcz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3pohptxdl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaorelgm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3oqmhkfte.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvhdumwp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3dpeugkeh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3zsyagwdn.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ldqjuoix.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dhbfizkr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yxnoumma.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3jxlhgned.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfbghucb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wdycfazd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dnwhkffj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zmkfhjdp.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3shzfpign.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ixevvqqq.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vravmjhg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hisfmpmq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uoymepps.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vwvbfhkn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3jboujrud.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3kugpmvtm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tsrtiezi.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3crrvsflt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3uhlakhub.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ocayqnuv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hgnxgukq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3xtktrkjy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cbftyrfe.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3kzobupuv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ofoadepn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwxudvgt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3lwsfxjsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cxvvofub.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ilmgbspg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3zlrthkue.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ggkhmcxy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3klxarmck.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hckmfhtj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3qtbalmei.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3xjckeayu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3bywnyhdu.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3zgstwmcb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hehqnqcr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3imqquhsb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3jvmzefln.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3vucwvwhx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3vnqtytvf.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3eidamwku.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3bdlarole.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3jbdcreuq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3appqaeml.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3tztmtsmk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3lqkzzzhq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qajfhndt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qeeksztx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3netxezes.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wxhjxwxh.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qwsrjecx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3rmtxxrzu.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3hakwakuq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3hrryhrtl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3glezrgqa.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3turyrwvb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3lvshdblb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3aavxquaq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3kfolzdny.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3rfyotfax.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3lpzxxxfq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gdjrspkw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3sxsyxpgj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3smmtmfza.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3reiklbkt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3qrotkkzj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3degdrapu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3oqgpzdmp.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3uexgvgzu.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3nbzwucgt.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3zcegtism.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3pdzhsxgl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3vhwpsade.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cfmbemut.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3sjuuraed.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3posxvdtr.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3vaewoibg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3enwebypa.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ypydcnhg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3lzfrvnjg.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3bvcqrwut.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yzfqtckz.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ipbsvymr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ohcdwcep.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ztygctwz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3dcpzwmcc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3pkfpdmph.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3pmjkewuy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3rkyrxlmh.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3djadxcya.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3swlhhnci.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3pynxevse.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3pwvmcfsl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3fiidiebd.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3pwtugtzx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3owtszftr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3yktktsrz.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3xxqqmepq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3wymzhcmi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3xfpaylqd.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3lwdqzxpp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3hdhqmjsl.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3erdansrc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3dmxywpht.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ydzarmdc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3cwdbkjyl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3bogmfdru.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3cexxffge.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3zzicpwxj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3zcdvhxxg.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cnmkehxx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3rlyltmyy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3bydsynnz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3bczvbnkg.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ckjipiqx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yactlsiu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3pcfgzgvj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3aohhahwb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3bqbaxyde.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3nkiwyuai.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3vxjaahjx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txwvrhic.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3meynntxt.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3krvptgub.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3orzcdkko.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ctuwbkmm.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3rphhxdfn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3tlbtgneg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ljdjlrkl.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hmefnjdx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3byzzmukf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3sdvlcgim.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3psoeurtc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3kycozfrd.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ymaojopk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xrflceld.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3fytvgnwn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xoteirug.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bpisungp.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3opjhsxwj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3kfwpynjs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ckozjakg.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3bhkglihk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3fkdegsnm.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3kvhjgnct.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3aqeewdge.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3drzxpiny.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nqoxtjnb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3hkmkwnwc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3jncdjnpb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3rlybmhwe.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3gcqtrasc.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rofsoswz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3lglxxpqp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3scuuwujm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ybfgsiwq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3bmkgupjs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uhurxnek.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3rgasqsms.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3gfocrqmh.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3jaknusyk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3tbfnkyrq.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3vuyxponv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3obmqicba.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3okbzeeob.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3fdnejpre.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xsrqbahx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3qrgvwxkm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3gwwhnehq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3aovbxrzf.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3rbiahdha.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3fmfwthac.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rtvslgkg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3cfggykhf.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3uhffnhcv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3okwfykbe.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3iykmwkhy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3bjyhspta.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3xbgivyuy.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ztybwzvm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ztesrslq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3mtxqdtvv.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3rymkphoh.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3noncccdi.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3nxrxpioz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3nciyrmdx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3nctumoyt.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3hzofvioc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3jrhzpfyt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3uhvwaisk.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3hxpzjlfs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3fnmsrugp.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3rrzaixsw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3uqvtqutp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3qihofenw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3oicxedhb.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3hveqrzkp.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3kqittsbz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ywhzgevl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3qvkvykqm.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3eeoqbulq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3dfwwmlxo.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3mrxfioid.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hhnudbvr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3oviivbni.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mqcnqnzs.html


<!-- 参考信息 -->