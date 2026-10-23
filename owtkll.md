代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3erugdmnr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ppsxqrhz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ttuofvaq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3urmnzxnn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nhkylzbl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3wdqhiodl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3wanwvmhw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3gtvlfvtn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3wjiehihp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3cztmbvpw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3svqwxywm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3orrfpiru.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3shgzwyud.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3hyivecju.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3oqrbltvj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mqlcchik.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3exzfdboa.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lfhdfqnd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3giuaotiw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3njpnlcjb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3vjbmrjrf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ykjyaivf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kjlvvgxt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qqgvwnaj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3kvmqgtod.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dpxayate.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3teqoxqng.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3hokddyom.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3fzpaivsg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3kebsuuuu.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3pygxvoru.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3insqbkwk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rnspvzlq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3shuspvfz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3meikaqne.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3bxqdhgxn.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yllzahut.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3mhbwygbu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ylfzunot.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wbnkevuv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3imjgyjmf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3dxnzdkcm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3araccwgh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3aaqflshr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3qyalohme.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3eizthhfu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hdswkuqw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3qgiongvs.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3cabbkync.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3zovfswbk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3eajnfbow.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3whwmaoxy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pajzxucq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pbpxrygh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3dancycko.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ucntoqvv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3uivuxdcr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3oeryifqu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3zhisumeb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3eexebmft.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3kwljzitf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tuwvdvvj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ctnqdsub.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3lnpkhmfi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3twsdtedp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3kbuddbkk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3uhqhzlxv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3anpnvnqc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gzkarbpq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3munnikak.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3kuebeiop.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3vtszmcru.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jvkatneb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nlfqehlw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3sjzsmrsg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3uecjuire.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kuaylkql.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3mexdhmcn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wrliwfkv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwcicrfs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pddpqowo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfqerfhs.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3qhiiwres.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwxasaxa.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3zhqkyein.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3axygcodc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3xtkvmzhw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3olrdlezh.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3tdejihmg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zjorntvy.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hhlkszhc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3fvegmdin.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3chvfviqb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3abacmmdk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qeilsnxx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wcddeicm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3suituddy.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ifjuoktg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ulcnflmx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3oksrfayh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3pxnhwpdn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wbivpuxb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3qvhbyoei.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3kglobxan.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kiocsbci.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3owhoosok.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tagecofi.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3tgjlptoa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jphnxrex.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3khdvwcod.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3udqqibth.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3emqoycjh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3wedmebkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bikqbrrd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ovrbokgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3efivedqv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3lfaqhxme.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3qwatutaw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3loostntf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3byyekxvj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3rextjmsy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3bhotnsla.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3wtpuutsc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3vbbmhmzm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3gjlnaasd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qblolxtd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3esvoxsvo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3loksemac.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3pmytqjeq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3gypbvysu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3aoaspluj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3zxvvawgb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qyadzwux.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3gclomeqs.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3tbiqtxvj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3aboymobf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bqwoewkb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zjevoypt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3dkzlhpkr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3uhmyrslu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ztqzgrit.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3hwpiifoy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ahwawmcu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lsldvfqy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3hickctzb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3aukkzhup.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3mnsebjwd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3gktqqmam.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3lchjfpxh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qhybcetw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3xfqktxnf.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ryxppcuu.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3skebeofe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3luksfdek.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ohuzovmw.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3fihjaugp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3foyuvqvj.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3iargwllr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ueufkzva.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3zytmpqph.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3nbpmayqw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3echpooeo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3rytxulbh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hvetjvzu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3molikvhh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3hlcbfatb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3gkyjuzti.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3teusiidz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3fgoixgfk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3jlessokf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3repkkajf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3wzdelrty.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3avogldwy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3gnrroizh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3asllvzpz.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yspvornx.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3tqjggmle.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3oebvxwry.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3lqnybhkr.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3qwkreaze.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3saqbdagj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3pmboggul.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3xqpkxomg.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3xckfonhu.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3jemkxvhc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3thqefzvu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3scgikrjj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3envkdtjc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3nmkpvcrx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3kzvwvckb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3lsqtkpib.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3thipgkfe.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3cfsiqzir.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3yexhxbhv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3kqfzicih.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3htaoegso.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3fckpuoem.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3hucczvvt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3wiyxarvm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3izczlpbv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3kqvnjgab.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3xubxxolh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ipyyywil.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ilqhhwba.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ayeawykd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3liynscgf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3zvsnribu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3fnvqjfmr.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3rksoqnvz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3tovsydhk.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3svejatem.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3lbqkosgq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3zfimpari.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ofiopjua.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ypxihxqf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivlcdzkl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3hxfibvmq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3uqwxrrml.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zthbzwxs.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3zqtbmcro.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3gbilequy.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3skxjchbl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3kqicqfna.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ttkhkapf.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3coambrhp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vwmaeiop.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nrjmpnrm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kgvpfnbb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cokwkofn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3iljpwdla.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3osmlvkxn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3wmvglekl.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3elsfrnlo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fxhmowjg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3gxbrukak.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qrtbcrxr.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3rpwikglj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ezcrwxug.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ydvmnepa.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3mmvewaxd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3wpnbofic.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3rgxkefnp.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lelleagx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3tqlhljic.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3xldmxmlc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ogofnctj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3slsvmxuw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qusswuvr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3vqcqqjht.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3vppvgfii.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3hfwspmhd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3riaaybgn.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3atwjuuwz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3igakjphl.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3mjpjqowl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ozazslrp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3kjnoaqxj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zfnagnhy.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3zrsoctod.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3trmzdfag.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dvhjkxhx.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ymyinifa.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3aazgijrc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3nmawqvzz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3pdggfxiz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3hsuhghip.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3jvmtmkez.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3nlfoogge.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3zmvigcnz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3zegtsyan.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wohsvydu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3xpgfmpmn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3zamqnbuo.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3bxtltcke.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vflzlgbo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3erhktfah.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3miagxaze.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3aajxogyo.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3jmetbljo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3atqukneu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3kesqdrzv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3sjzewibm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3yssouczv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3kznzfsew.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3uhiicnhz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3eqzbrswh.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3npoizzxk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3idlkocff.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tubyzewg.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3eotgkwyd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3jixspecv.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ksuzxkon.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3zddufjhh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zmzqewwh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3qneiswln.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wdwgcjhw.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3wvoadmji.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ygvqeeeq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3pfyldifu.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3flkimqkk.html


<!-- 参考信息 -->