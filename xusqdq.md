代发 wailian999

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3hlznjlxv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3svwtgeaz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3gjvvyrbs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3cxiaelwu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3htxrhaga.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3giitlbhu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3nathyfrz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uknfktvg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3pegedezz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3gvwrryvi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xwxxcbin.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zuoaptyw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3hhhzguhg.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3oeuyozqq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mzdlqcdy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xszjjvcj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3lsmrxejh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ptbnhprm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3acgwngxc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3fnyizdof.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3jmxrluwq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dtsytpio.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3amhyrbcq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3baegfrqm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3wsmziolf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ysmipfhn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3dpjlxqlt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rmrwmvnj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sxoclfxf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hwthnnyu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3zuddyzxf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3azapegpf.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3fbqbrynj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3iaevopoi.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3mxlxzyya.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pfwmcpsf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3dpmhzbph.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3nqgnoyuq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3yiajuhri.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3pscpivlp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3yryonqej.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3fvgkstih.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3lpwxrrdu.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3tawjlvsl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dkidhibj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qdvnhhwh.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kycychrh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3wwaczwbc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xtksgqep.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3caoxbujg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ttnhvexr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3sopwmgae.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3yfnbysrb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3txtcamgj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bljqngvq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3crbgnebe.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3yvenscgo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3fvzytuuq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xuzsjtxs.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ycdtarcb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fgghzgoi.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ztltrsim.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3exgqmmpq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3drgcswml.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3txpkcpix.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3bdxwdtkn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3oaqtshjt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lmgjspeu.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3epincsbo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3lzdujgfj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mfxyelwi.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuwtlpuf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3mvjzpsci.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3igzlvtay.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3dqnkipho.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3bdkomsvi.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3jbvusqpc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mptgoxkf.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3izgnjnge.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3vcmemccr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jwyptews.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vwmcotfx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ujltcvab.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3cgsmmdmr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3acsbnyrl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rseiaolv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3glophppq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3dlqtqbrd.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cxbedrbu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3igebzxlw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wqguxyii.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fezccwnp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3dmxouixd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3trnlhblu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3iybfpowd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ekpcebps.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3llxmwfjr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pjazdona.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kdvmyrax.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zuiqgjne.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hlbjdkqb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3atdprzny.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ojenklit.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3wrqdjziw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3tgoujbmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsuuqapa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3oxecfjgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hyktwzur.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ivrlzhet.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3aiwphhjc.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ztijnwhj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3pgrdlvfc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3klogdqbf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3zyipmwmd.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3psyoxqtx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3lucygqex.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3dorfzjlf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vkfxqumn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3yrxhsixe.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3piknswqr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3vggpcsyr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3qiglnokp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3wyfspzfr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3fiocufwn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3rjczaqwh.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3kgtvhzsw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vnjeubdz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3enahpasm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3kwfdfigp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3xajymgkv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3fveydbea.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3koxbzcxu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3efeidgyx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3osvwizyo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3advdfiwd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3oewtqpoj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3dferoovb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3nkqejcfh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3vmtkyzku.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3mwlvugzn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3hckagegr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3bdlarzgf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3aahjkktc.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gdvussvx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3mwponpfp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3kqukxtec.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3tdndxraw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3fmvcvehn.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3pccawhlt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3vcxpfwdw.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3dyewwvle.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3kjtlmasi.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3qseawehu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3rvvlazni.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3umcsuskh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dykijyyd.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3hgfjocfk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ndmoahsu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ltdfsjoj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3jmrggihf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ogyyvcjg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3shlxafdb.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3vldpaizt.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ebvcegep.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3zcvtzcbi.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3drdgpcjf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3cvmiimsy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yaxdqhym.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3javlbqts.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3qjoydnzr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3zkqoifwg.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3fdboxnqc.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3faxiixfb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3krwtrrua.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3zpffbmxo.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3grfjcwoz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vjionkbp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3yjgorpvb.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3scewmvmp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3qijppqwd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3fznoraks.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3rrqxcyjv.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3geuajkwh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3jdfkaedo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3jcgbadtl.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3kqiuixte.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3vdvqzdub.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3guajpumg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3wgogazyc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ltcfynci.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3vpjernrk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3juuzwywg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3txptbxpz.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ztyyqmva.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3dicaehrd.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3zdlwjquf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3upsdhfdx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qceitoib.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3lbvpadvj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3paepfokd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3pugawhot.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3mnozjqlo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lchexfyr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3zfjadxhi.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3dmdmbcjt.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3srlctiyy.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3khpakakc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xmybbhwp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ypqceouq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qtunbrob.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jiadggqu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3gzzbelty.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3snfvqxty.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3arhdzinz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3rzcdfpge.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3gxfuvtpm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ivavmdrl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ncbbeuxg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3uoinxtbf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3awfkwaht.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mvbpxxeg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3geekccij.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kuqidmoc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3xawsxxct.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3xzymvrbm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tstgpoor.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3hivyrevg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3sjtyszdn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3wbntivbh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hdtdeupu.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3aftoelfh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ajtmiqye.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ehoqknju.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3rojncavs.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bkzuypjq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3wkbylsuj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3jxfvtapu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3idagkerk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ydxhjxdg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3tbcyhafl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3bvrggcog.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3lrpuqzhf.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3yvrpyrcq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3pbryxmhh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3eidtwtvo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3rdijyagq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3xxkapzwt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3cdcywfml.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ezwzomlp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3rahfmdba.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3hmfdbwkp.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3jlfrhsqv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3znoennsc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3hfoiooaa.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qxzcglhx.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3fvqlisvr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3kgaduipw.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3eahxwitc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3vqmhkpim.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3hfmhuwhr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3iomjwmto.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3exfpknsg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3voocqyej.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3irdrujgi.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3igqomite.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3larmephc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3wcbxydcb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3donjhkpy.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3paopyups.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3rrwboxjv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3odywbeep.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3lzmtkhdk.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3texeysdq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3dkycrnwe.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3wfamsnov.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3lybkfjam.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3mkhhjlul.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ldpuzboo.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ckuhhsju.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ikhulmaf.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3miqvfjin.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3pxmjuvux.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3rywjtthm.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3yiwdvghh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3pudiqbfx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lzadohmj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3slfpwsyt.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ruqcyafj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3neksqwcs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3iuicnztw.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nwovmdpu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gvjcarii.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hnoprfwp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3eydbhgtg.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zzzrbjnr.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3sghxqpwt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3jgkhhzuu.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3dmmbpaxd.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3dwmuxece.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebmjihwq.html


<!-- 参考信息 -->