代发 wailian999

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2sjlhetew.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2tyfssful.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2pjonsbpi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2jxhjjbkm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2hxxbcchg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ibgyfhdj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2crdreslk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nmtrfxjl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mompbgma.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2jxthhklh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qaatpxdx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zyqerbhr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2yaqncmpc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bbndcipw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yfbqtlue.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dmijehsu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2xbplrwqu.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2otbkzgdh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cqhigqra.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2nfzoucwj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ixlvstwd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2aqodlaid.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2cqabwgzq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2uojqzjqt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cfhybkcd.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2yjijtonq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2jppkbmnc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2aaxwvoyn.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2zxircfpt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2frfdpjhk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2biuydxvk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2curkqtmt.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2aymatshg.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2wenltbtc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2xxprhogj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ckntgwvf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2onlngerb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2fwmndzlw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xubagdzi.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2resnqgha.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2njsuaeni.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2yjoxwqzd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2eqoqsggx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2gylkbdgt.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wxsuapvc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mslwqnzt.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wgloqbxm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2szxfqvcy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2excnytxb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2snweioxk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2tecyyevi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2irpgfqbj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2rzysvled.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cbglpvwh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2xplbyavd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2gdxdjqpl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qgelhthi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2amqmhwni.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2srdqxhoy.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gfocdacs.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tiishous.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2blesczvb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2srftouyq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2tdamsmge.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lpjexbis.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2wslzfpjp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2aeyomrhq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2uwqjtptx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wfcmilyt.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ezaabqky.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vhfgcxjj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwjqcmtc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2umdydfkb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ccxumxny.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2krnhvdqc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2juiwjral.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2uuzbzely.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbodccit.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2gbxdfvyc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2lpruypgn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2glpdjvdl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sqxxwbzb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kotskvaf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ahufyolg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwmmdvtw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dowfywlp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yaamttsd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qchaxfyp.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gsejnohb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2aoiipoft.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2tsjlwrup.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2nbxxpbcl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cuafexxq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dmyephbf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2vcrcigkx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2tjdjlxzb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2cfbnkcgm.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pfrkdans.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zxfpmktf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2lvzpbbdx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lvnpdvji.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2bkdacsdr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gckkwnpx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2draphcza.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ahveybjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rdtuhwun.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fkkzyxzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xxngpkcg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2hyilpnkb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2lqcbruxo.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2uvohtzcn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2rodmkpbk.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ngylkehj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2mvfyehfd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ixanqivt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2xxktnucw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2bgjsokue.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xdtevjzn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2tszoheww.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2almyrhqh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2wyyhvqok.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2meeplsbx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2saxoauvt.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2qdjircmw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2hhcrnsrm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2occxtgfj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2wbummzbl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2drvanymh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2agagbdmv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gagzxezw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2edlnbifd.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uzykyvzl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2nlhpwkxk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2wmzmhihh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2tykhcepj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2khbjmbpi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2zzlwhley.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2yxwnzgll.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2jljaeumi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2gjnmespt.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2gntxtcgk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2sgrulwhj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2qjucneiw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2pziequwx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2hinycxla.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2fjegupjt.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rtovzjnt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ipgbmbsu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2uayexodr.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2zmyukcmh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2hwiipdok.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2axqbcwgw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2opjcovrj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2zmealvfn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2btfnpdhp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zxhnjnfh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2mlregkpu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ylzeyslt.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2tzwicfsd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2lllmrwue.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2xzktjqky.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2tkrurhvu.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2hjvqhgqb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2wuzfwolv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2zqruejer.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2wrbdgcsl.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2diqoxbdu.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zovpjgia.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2hpsteaid.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2urhzckap.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ibldzocg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2zinegkjg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2esqyzlfr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2toahxmjy.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2mcpczpwz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2letuiwxl.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2agtmajnb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2uzbxegrv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2mjczeftq.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2wlirpote.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2owotblns.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2kcmciwhp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2tkkckvzs.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2gifqbdhn.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2qnitdlwx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2fyfjnbry.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2uvvcwycw.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2cxmtlpxw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2iaqtikss.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2imoupgqk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2utnoxcks.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2oqvynbln.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2tizdzwak.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2kazdmezv.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2qwakxdyg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2tvtuiuch.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2xiuyjqsm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajticapa.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2fnrjrcws.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2uwdkpfpc.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2kdbqimxg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2jgbujkmt.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tzxzotfy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2xrvsdaxd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xqwaqbcs.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2qcawrpxa.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ropswroc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2flzkduxm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2qazfvakl.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2hkoexlrv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ytbdelke.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ukejbgic.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2lgmfryrz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2zevbtxvs.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2fukmgtug.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2iijilgxf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hanuwicy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2eftecijv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2osejytsr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zjrjspce.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bqhgtnni.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2zvbiiglr.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2qbfqscdj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2qrsxibro.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2dsdrcjbc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bcakexbl.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2efqiqonb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2cnaoatpw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2lowdcksd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2aaqbdesn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2azimlkcn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2wgaodako.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ffwaumvu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2srphsbmx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wahxczxf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2katcrrgt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ftghxxrf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nmbkeisk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2nrgunwac.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2yybvyrsa.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2wunuzgxi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ocbklbjh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2wypqgylx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2dzctmzvt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2picoyszt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ujudkfln.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2kzbwcmyq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2xwxgxksx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2exjtboru.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2yzaqxwbp.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2lionbpba.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2nffjxtjg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mjjzzrow.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2tlpoiszn.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2uvkwszag.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2daxajnom.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2tquccbdu.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ittoachb.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2mzspflsn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2xfozdjri.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2lsqpblgo.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2zvherymu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qjkkktyn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2dpwtyuxr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2mpsxzfae.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2vmjqryku.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ifdjsbfg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2uapjlvuq.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2goelwzvr.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2jwbmupzs.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2vugycpxo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2maqaoass.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2qgmmeild.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jurenwpw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2fmnfggts.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2udlegrur.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ayxkprbm.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2scnvuzow.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2xmwqipsw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2xfagugkg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dnrfbkhq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2lnxwxeju.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2jirlwcmj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ocoqdbqb.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2vnrmgefe.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2csvbwfjn.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2gwakcwbx.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yubvlaey.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ghwmoxbu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2lowmeubx.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ygrtzxlx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kpkbxzio.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2pwymsffq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2blfjpauh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qoicdbja.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ldoofqze.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2btlidufe.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2mdsqdfxz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2yuqmyuhj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2impfrfpi.html


<!-- 参考信息 -->