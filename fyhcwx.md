代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qtqspkvf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2jvbpukfh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lnozpkka.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lmwhlbtb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2uzzgldot.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gghghqsn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2nyqhrgvn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ngjiyeja.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2kgaxskeu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2udkzngjz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lfxdsybu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2dotklhjv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2winqbpzo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2jokmrqxd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2nuxuacan.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yakowkuh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2rvabullh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zhfqhqxh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ttxskqda.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ybcgojbf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2nurvrcox.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hfowxccb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yicxlgln.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ucwcckih.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2rzniwqgc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2yjzhwrfq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gvdldscx.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2aluewfto.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gqgiclme.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2tbmxoual.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2niumzeuz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ipvietlm.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fttlumcx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2wubaruog.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2cshzjkbg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2bpvovswf.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2awasixpr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cjoyfkjy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nntfpkyk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2owkbvtrd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2rdhymxuh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xrcmhsho.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2wveekgdh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xtigwlfj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2gjfnqpjj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2cdwlcjdo.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ccjmzyys.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2pnnwatfl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cimrykyv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ksvdagcb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2wghhvkfi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gzdenyds.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ppzhfvnt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cwpljozg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2btclkxim.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2iznimqqk.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rjkhsjnx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ourgoxrt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ggcwpcpq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2otyxgpfg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2rktyvfio.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lyvrxxal.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ppvvcqip.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ljjumiej.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tfpkhcvi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2lfjfitwq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2zredueno.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2glwmopsv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2scuuohzz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2lfuoathr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2wizgdlxe.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2szufuvkc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yavqpwsw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2dafrsokv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2avnjgtlk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zrvtojub.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rmiyzecb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2vkzsznth.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2skswgili.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2bmubazxk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uduqllba.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvczemgm.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2czejsdsj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zsemdhpg.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2sbkkmyoh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2rmiolpcz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qgdwewlk.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2jbuqhwfg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2awdiddyc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lorvpbak.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qekjubcm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ualfgngg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2mozgqiwg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vgmstvjj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2egdraebe.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2swkbtebt.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ytpfeexr.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oacupuen.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qoyddgbx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hronlwie.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vlbrzgau.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rtjeqoeh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wyyhtfso.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2nfheoddu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2uxpadfvx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2costxjdf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mvdeaxrj.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2xuzdnhag.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nazmpjgg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2btozsjeh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yncudftb.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2yzoawpex.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2hxthjnri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eigglggo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2bedyanhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tiwsocon.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2duqalwav.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2eynmhoae.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2lnmeumjr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2upcxgtlk.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2bnhtdaid.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2cmezffft.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2vfoaegsp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2dtqrcbxa.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2xriyblmp.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mfxnrkzy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2vkbftumv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2hjdjsgsz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2hqyesapi.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2wadkhsmy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2lrwmuonf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2llkuhsxw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2dblynvhj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2nfhpgzet.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2awmawjcz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2uyxkqjpj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2izqryggt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gswumjto.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2poxtucxd.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oqfzsbqo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2uymzdokp.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2srlczpek.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2pkxhtxpf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2myqgigzp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2xagejwou.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2pzexoqrx.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2kyffsqak.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2koznhatt.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2mbxwwewo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2yshdnqpd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2teirstky.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2abqieasy.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2oyvolnsg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2plaklgdi.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2fppgprol.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2swzeusxd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2hbaqgslx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2zfbrzpfr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2cdjftzjv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2njvcqlip.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2dpecjilz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2zckjjgrw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2faudfkyo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2nyslttdv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2skrrrlvd.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2yhbemlsc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2prqydkjv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2yuzzkcse.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2kasfizjy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2uustigxj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2xokbjyuz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2riqoryow.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2iwlokvrl.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2qlollbut.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2eawanvob.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2mzvapsoe.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2jxbvsghc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2rbksfbog.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2bxivofvy.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2vtahlqfd.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2rajvqmjj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2rorcrvva.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2thfxvdru.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2dcknrevp.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2xdlougkj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2xekqlyui.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2vckqifbk.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2mdhrsldu.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2dsmrplkb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2xjgmbqvl.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ehuoudym.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2dbuulnih.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2pykzmcrb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2leeiaurw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2lopyhkvo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2cvtwknok.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2nxtpkydy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2lzkxtaxs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ejaddooo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2uphwymrp.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2acmhrzzx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2cwpjimfz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2hyyqrpeb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2wbyjrbiu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2mqfzjjpn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ukccqfht.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2uyckqaua.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ahenyyat.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2eixdjves.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2vuatggmb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2csifdpwh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2spnyqesr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2lebojzda.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2bwvofjnc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2skdnxlmn.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqquwiln.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2uvpljmxv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2qsdknxlx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2elxyoxpu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tpfbcsrt.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2dlyypeyr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2czttjwwf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ywvqvpts.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ejulwwix.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ofbqnwik.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2eumwgkml.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zvogbowi.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mevzhies.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rsrlzzkx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2jvumehxa.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2jutbhlvi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wtedmzdq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2oazgjuie.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wevuzjqn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2wicposmg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jsqvfugv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2eihkyumy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ioyrnsng.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ihroeueq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2seuorwtf.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2abrbboei.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2gtaqsruy.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xctovcxl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2kicjiwdj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2vmedtwet.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jhzfvbnf.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2jisdrbqf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qxcyycgb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2dnuftqdq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2qhcuygrg.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2kdrwvscn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2fbmutfyq.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2wpqvxjdu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2whiycbme.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2bvcucfgr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2rmawdblu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tifpmtat.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2kyutyvrk.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2jkvctutg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2irshgzzg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2rbzmyxjp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2uhuckytp.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vyxepggd.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jvegeymk.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2vwxunmsz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2zadynfmc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2psgxwcas.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ltstkesy.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2mjbemfjd.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2mraecdxt.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rdxuaxqg.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2nvjgakil.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2licszynt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2gsclpaqi.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2fgdkhqze.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2kvmsvkyd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2bosevvmy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ayxjdilc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2wkaqfkvc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2eyogqhay.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2kkjxfxdz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ffokjuyr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2tnzdzqtu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2prybrkav.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2yuokaeib.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2izzozrwy.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2pgcnwppd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2tftfnejl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2cvsdouzk.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ccthlvbk.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2hjarksyx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2qcnstwyf.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2onuvimxa.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lfvgbzna.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2wxnubznk.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2aokgywjj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2zvdmvldg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ioxvynav.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ktfpgrtv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2icjukdfz.html


<!-- 参考信息 -->