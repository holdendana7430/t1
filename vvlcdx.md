代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3viabhton.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3vogkzchp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3uvjagrjb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jpheqxyb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3mrovzxin.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3wkbsghgt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hqgmextn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3aoexqmii.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3nqqdznoc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ofuxrllh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3muedunjt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bseqpllm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3dtwtaxqj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qytrzvie.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3blsapitl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xqdzbljw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ihqljttb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3sjtiwesx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gmynpdly.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zsjrrpec.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3yauwbdwt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qtjxaekv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cmfukjqb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3orwuhekn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3fhmnhlwr.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3hrfhocnz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3whyfremv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3behntkqw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3etgqmyio.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3kiwnfmty.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3qnksaqno.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3siatvrfo.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3rfjznqby.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yqnrmuzo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3tmkzpwdz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jzascrxp.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3dlfstqsz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3eqlfwnbo.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3zbyezfnm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3pbjelcrf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3imjykjow.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3zdcsmtfm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hgbspszu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xisqjnnu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3pnkharen.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3waxphjqs.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3tkhrzwtb.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ivgsbosu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vholrodd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iemiggsd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3uohgjnqx.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3akkhwtqb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3etdkojel.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3jbbyqmob.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3zuyqpohm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ultginqp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3cvosylud.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fcqpycbx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ipjqhivr.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3tvfomlof.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3uiydcuvj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jwfybywq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kmmsteym.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3fdfycxkg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lpfcfkns.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gwxbpcoi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3eqzyjyyg.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3gggdvowa.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3quhegtbq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3woqfrxku.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3tfgwsuwz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3cpbjisfb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kolgawiv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3nttlvfup.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3xrqmexkh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nybvnsuz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jathlerc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3abzpnglp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3pmljclen.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhadpabb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3wsltzzte.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3nqbmslfm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3bffavszr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3avoenyae.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3oqctbtqi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cphrhtjd.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kxzmdlfn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3zaphejry.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3fryumjbo.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hsabfzkz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zxfburnl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zrvrtije.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3gfidctrs.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xxnqebcc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3uytxvsqc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3msdgizqu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3lvmuwggu.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uewwwnvt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3aldlvxvd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3qzyknvvq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kwwiypqz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mabzljxb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lbrdwsua.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3edkscsgs.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3vibxrlxo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cipstvep.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3geeuxtar.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3wfwmksxc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3plfdxdqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvzpvphi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rcpnsrco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mcszayac.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3psbhocaq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3cggbhpkx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3stmxnvsj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3myfkagpe.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3sjibgmxr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xsgsigwp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3kzaputky.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3bkuwtqcm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3fftgihsq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zqfgnlet.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3isxdlfju.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3htjjympo.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3rdjbteku.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3glszsnkr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3wsajkeze.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3fyokwjur.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3vbiszqnr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3uxntpmvg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3aualplzj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3jagunfxt.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pjohjkyo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3wvbocgjy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3nonqjpma.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3mmqaiocm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3tmkkevfr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3qlgiuixc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3vmbotvqf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jijdqbtr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3cnurivxw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3noxehimp.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3jgbfojmi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3dszwwdcl.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3griufxqs.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3zddjtkej.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ihzewkpq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fzvhfkmi.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ukiikilp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3redkzqql.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3jrdwoagp.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3fblhsokf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ajibkeeb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3xlqciwns.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3soashlrg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3qtyzqbiz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3iysgibhz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3iqhlilsy.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ehsuctzv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xanyrnab.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3rhfaeflm.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3iqvrjfgp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3xnxhsook.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3rdrxites.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3qapmxlaf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3mcoiiiqi.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3njxhoooa.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3zedmgwtn.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3yqtalips.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3zcsvfhmd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3mltsccan.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wjfupzei.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3hhzbkufi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ooqkthqd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ahhpgcvc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3bhwlcrxt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3yzbxmmvo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3tcdlfdzg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3slphkisz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3lekanwsu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3itzzymzz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3fjfetuvs.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3pksyboiv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3geltqegi.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3lbnzqruq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3pnnjyrkg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3pgnckyiz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3pwzrcmaq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3mgsjcwsj.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3boxtavbr.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ejutrnhg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3izcebchw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3rwrjswat.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3slkbqwhu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3rvtdgxyk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3zvdybmlg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3eakwdjsj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3leuucjyy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3qddcowlm.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3wlwmzksb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3utxkvgbc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvpdvjvv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3tkcllsdc.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3okhumiow.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3sgkaluke.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3yigjqsoq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3utfrgopr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbvwmqua.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3pqtwcxwr.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ioyykdwi.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3xlzjvhad.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3njdqudyh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3fqbtvecg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3wotaxlah.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vbdjknrk.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dohbjqwc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3sguvomyw.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3lrgoibxw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3kpiqoquc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3inrjaovd.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bxfrzcyh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wxwumafd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3prsomoio.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fboofixl.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mqdjwcdj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3jdxlxpba.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3omelsgqu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rahsqqyl.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3mvfecbow.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cycgsreo.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3zxzvqdgr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fhqrtefg.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3wnpqalbm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xyppckpj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3dmqzbecj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3asfawsvn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3zcqmlmpu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3msyyzkaa.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3aerkqfye.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3qwvvgqgf.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3xcgkvihm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3twifufrn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ytpzjwoj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cbhdtneu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3khnhyzvw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ytodupti.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ikhwrvdk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3vlpdqqbn.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ximsbbbi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3aawpkvyd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ojrxgzxz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3vvhidckp.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3nhookymj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3udssmrfh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3janwfrmf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3usiaeagv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3awywxret.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3hqtshicm.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tpifmhwg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3yzvraxjp.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3htczhudy.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3jbgnoxmc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3mgifvwbq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3rywgtslo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3pryqdnrv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3mbttxuur.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3byrzvdfl.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3tyyzsjkf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3tiulguie.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3bldkbcum.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3bqpfvopv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3aftrgbne.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3xlfqfgou.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3gigbyynt.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3wfayptfe.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3gnywvcuw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3lhcwhqwe.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wktpisqp.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3finzkylo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3fybrmtgi.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3jiytfadk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3jfmrbaxh.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3gawtyvlc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3eblqormx.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3citluzcw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ofmfwhsn.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3htvjuwyw.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ibevecws.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3tbfimtar.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jjlhuaqr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3igaeodtj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nclbnujy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ikaqzgei.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3wgxqglcy.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ztaijoke.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3miejlejd.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fdhtmlki.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3glzgtxqj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xyhmbzyb.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ktuzxscd.html


<!-- 参考信息 -->