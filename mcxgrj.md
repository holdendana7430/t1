代发 wailian999

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ockcnteq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3mmkxrcfr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3esmkkjlh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qfladcke.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wuoksclo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3tbjyuwjj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3fkmtwrji.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sbwsdity.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ltsewcvx.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3uusnocxy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ltmzbnrv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kwwjbcsy.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3uqzhkibh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3aqkewuzk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ovknupgl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vzplcoqk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3fauhdltw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3oprrufit.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rrcnosls.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3solqkkci.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3momclnjz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3fohzayvj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hhbhoiym.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3usyvcbbm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3hjklrzal.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3artwzdld.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3fpuftmpd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ibvmjwdp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3zsifzgmn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ngscqgyv.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qswhrqdi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dqftxjqh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3lrvwpobd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3hhxvqhfe.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3tjrbedzm.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vlzoszhs.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mgtidbas.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3eurezmei.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3awegoncc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3quunmisi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vofkekna.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3oulxgqcf.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3dcqtqegt.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3uplxkdme.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pxthcqkl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3izthxxby.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3vejrrrrs.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3bjimbhyi.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3puhiwhdt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3xikmhats.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3hpkoxkid.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3tmtbbvnc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3oyazwono.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pcgibjzw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3mcgqbcfg.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3uacdfbiv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cicrufkp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3uqztcfcf.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3fobfhlus.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3hjoentlm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qhcxdczz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3sfsoedmv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3kswzccvv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ztirnrbn.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zcnuxrdk.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3kmijfbft.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3lfxdogpq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gtckjefu.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ozkhtlqd.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3tdpsgxjn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3hzqkeblj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wionmoyg.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vlhzxdhk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkqohfva.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3uuqjjyzs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3gurmfdvu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3gjhmpwon.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ujjjnjdy.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3qfkipkuf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3nycjffhw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3hddxydbj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hybpsqux.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vucesqbn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3towrplyw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3asraqvsb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qdepsqkj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bqttgure.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ieniqbdq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pbjgrzrc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zbmzgbrr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rybkiedu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lcibkllk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3mphfazla.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3icrtgrgv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vutixttw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3jylypgey.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dzkmjujz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qhebkodz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3kvvpkvxk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3cajfpyvb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3eoddbdya.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rrruxkgt.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nmobtoxk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3lbqgkxlx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3yspxbvpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqjvxlqx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3oyjgantt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebbfltzp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3njbrzjwa.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3sefgcykw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3guxnrlbs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3bwtfmria.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rpsqbtsi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3znckehwu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ydzsutzi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3lmnxbeiz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3wcwwhxdw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3whrmligx.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3mcbfbqjq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3cliaeqts.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3gycitlya.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3anogvrmw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3xdinfmdu.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3lxpmexpc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3lftibpjb.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3pprkxlbd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3bedxiqtf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3yjjvgpdl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3xygozxzi.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ylabsavr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3arztcvti.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3rmswaqoj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3raibgqik.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3cehlgfua.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3kklcybfd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jgiuzehy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3crtzspct.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3aqiwwjnq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3zuxojfog.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ihnlbtpr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3vsmoawhf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3bhilxsqd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3jicsmwqb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3diiodpvh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ezlzldrz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3rnbxitgz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3inaswjjq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3wtimjono.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3boapgjin.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3jlxpfmho.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3lwepdyfi.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3fltowomd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3fqmfdrnq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3atjuzedm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3qxhiyomy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rpsakamp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3edbfkpaz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3atpkjriu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3rertnpcd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3rrmuihoa.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3iuandgez.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3finrddcq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3wzwknsbg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ldkjgnvv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3qpucoign.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xjtskdrz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3nvarfqyt.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3xhcrinoq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3nulqctzl.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3avehxwtq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3gzydpljz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3yoydchtf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3msefienb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3skcslaso.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3sxbmccoh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3lxvwurjt.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ukaixjdb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3gsnliidc.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3yqbokaew.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3qeajnhbl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3itzuuzzv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3dzerozcu.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3krgwkjri.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ayisscjo.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3celbiptp.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3uzbswasm.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3wwofqfik.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zxlrkrnu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ujrathlp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3xdfmqlrj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3zejtxklh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3iisepuoh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3qwnwtkgh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3etnxsnrd.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3fzpixniz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3uybjfufg.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3brlakevs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmhgiupu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3mfnslgyb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3pnnkirgm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3puhhwkpk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ckidnnil.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3nnmdxaxa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3cwpeunuz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3dgrtmoif.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3fjpvylid.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3yatclsoh.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3bcwjdvlc.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3mjxayckp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3nzlvnypd.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hdhjxtap.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3yynrzpqs.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3qxhaukkx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ocmjndjj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3owxchahz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3xwcoxvgz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vickrznr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3eymdrhxt.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3drcvewhn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fzcvwtrj.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wrfochpx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3rgfeyzgi.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3avlkzqzj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sbddxxjj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3nwyiegfr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ropjwjhz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ycussyph.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hqwjfnjl.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3vnrxfjhr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3aqxnnubn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3umskiiov.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3qnktzpaj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3xtfgaxff.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3asxkhzle.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3baszsbxw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3pbgumewz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3gdoitlan.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nncpbkrh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3bewvoaer.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3twyyyrgc.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3kysbvmos.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3xxhflqve.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3oovrkzns.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3kuyrbkvj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3tlpgaxfg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3mrgjeurw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3veqgnaay.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ycxvnqol.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jlnsnuay.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3drqkpuif.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3chbvoaka.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3jijmvqcu.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wkghdxag.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3matyqqpa.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cddokppx.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3fdxequdm.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3jdjhpzdh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3jsfbdtcq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3zwrmccol.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3nhaezesb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ibuodyid.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vzrstptl.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3hlmlkmds.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3hqqhqrrm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3fpvepypu.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3lcbeodmo.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3rukvljxu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3kstqaivq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ogajwkyr.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3nivdzjrj.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3sdxujrsm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3awibzafd.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3opzlamjo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tdxmqddi.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3eeuhdfgq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3nfwktyzv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3sblxesbq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3otphbdzn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3mupfconu.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3wyriajcb.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3eadlwasu.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3dmvzditv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3nxviwcpx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3jbmziboa.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3vpashmzv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qfttvozw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3liexyjxv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xsahtaln.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sslljkbj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3zdonaiin.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xytyqwki.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3evkgqssb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3nkwpdeel.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3gknypxen.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3eiaaqsmt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3okvmebxa.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ywfxfvjm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3okcxunku.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3jdrkpyzs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdzslaio.html


<!-- 参考信息 -->