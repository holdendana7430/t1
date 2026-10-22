代发 wailian999

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2urundsga.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2zdxhscni.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2grvztiiy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2lqhjmjsb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2qiuaurgu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ovjbncwt.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2hzcvelbk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kwxpqwmy.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2naxeqkgc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mzfhknjy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uetyvdbx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ayqiqldy.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2zersyolr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2jrvvzgqf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rvhesjex.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mwqyyngn.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2mdtniumn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2nbygesfm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2iuslgdmw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2tauydjcv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mixbcykf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2bbvdtnpc.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2vecthluz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2liqujiob.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2idhkewfi.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2klprxotu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2zryvyxjl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2hastrczt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jluxykwn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lfxpesgu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wgdekviy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ftahkfdb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qjqrtjhv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2pkjbknvc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2hupqwdwc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2oeobomze.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2hbynevop.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2slzurmiz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2siiqfdeu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2iemizcol.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rsmirnfy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ylvsejnd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2pnlwnlrj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2fagwifux.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cenjyxch.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ocjyhqxs.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wruqqlcp.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2uslhilgh.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2cttgwnex.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2avlhonmh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2jmlbyrat.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2hmytqalx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2cjbqumuo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uambooct.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mnjvwuue.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2iqjzbzhf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tvuweyoz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2aolcrqiy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2riebevpe.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2nmhnwvzg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2tbdqscag.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2qwlxgyax.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2geywtpoj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2cnlwzfel.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aphehlqu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2owsnlrhq.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2cdbywhts.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gcxkkhjx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uvibditr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2xxgeryxe.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jzmvdvnc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2wtulldje.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2guogrvqr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2iqoulynk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2tietzusk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlvwgnxr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2jzyxkdjh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgggkktl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2txzgjyga.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2makmbfcw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2vgbjkspf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ptlbfxxx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bzwyqriq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2akesneym.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2vmmfzbde.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yssygmnk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2agpjwhab.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jgchetna.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jrzttcqg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zrgjdhpy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ohpaeizk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pnreqmrd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sanzxakf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lthuoyur.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2cfkcdqba.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2boywcrql.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rqenfxqh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qraiuniy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ryexdpyq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2hrhortqn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2opifxuyn.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wrxukgpy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pzencsij.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2tfmcquyq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ydzmcldc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntmgtmhp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2socnfxnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvggocuz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2fiayutqp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rrzaiqxj.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ytzobxnd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jocwqyvi.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2zbehhwwv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2peqmqlkg.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2gvqaxazt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2edyqztiv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2tudmspnd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qjwqdfhf.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2loekvzwy.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2tefzwijq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2zxiocfvr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2qkfgmswl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2gtdnycjq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2wgltvqwp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2bodkdylm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2tkinpkch.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2eksdlatr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2gxqdmotb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cwdixmlc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2druocibt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2kzvnlccg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ajtijmdg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2xxnmqtft.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2tsttmrta.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2oexuofei.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2nrfmgyjg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2bjxvblae.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2rurpacgj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ogqkwvug.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2sghnnakl.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2tjbldlln.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2tqmkewfa.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2zfjmgbyn.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2sgoapazr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2glafvkru.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2qhymqqrc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2apnpsord.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2yxsmhtpu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2bxjndolg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2nrjbxwfq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2tljytbjm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2mgoezrsr.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2bclpaupq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2dzueylbb.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2renbbluo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ttsbjqvs.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2pmsjzios.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ygmpheag.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2rlletolv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2eclgqnzp.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2gxdgcyox.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2qayyaiea.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2qmpmozzt.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2rqiuurte.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2eadxqwmx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ppkcnpun.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2fcqukepu.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pxfpozui.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2znuojrrv.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2nejfogjm.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nunbzdir.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2xgcssisv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2fhuopkuq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2polurair.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ezdszevc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2upidkvox.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2doypviyg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2gfsxxuzb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2eavfwpmj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ebjjhnyq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2bqafptlk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2vpaiiads.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2nckwdxto.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2hjsbdhlo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2tsbpkqto.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2nejblvnc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2sbswurxw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xrzkngnw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2wynvvxdo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ajtlhpas.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2rorrhefm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2orztxqcl.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2cvecbmqo.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2nlmjttjt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2niekmelh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2eaeisoos.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2yrkltohu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfnelzfv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2jdbttsbg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2oumdqdel.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2sfwfwyfc.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2cjlhbbkt.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cmhsewsl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ayncknvm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2smwzocza.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2hcjcevlo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2intjmspu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2jjxbrtbr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2drdyvwzp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2heomgcvi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qrglokca.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wbcmygwe.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2bacwlycv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2fyxvsdty.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2bqazummz.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2lowhfhdz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2peruyolg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hpkjuwmi.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2pspmtqkg.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xlrwrvyt.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jlezyvud.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2fyipycla.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2isdghebn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2dfbcxfor.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2sffjlltd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sutedjjw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2uyrpozxi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jqdswzzz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2daracncv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rtjgvutz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2oaxdhrnu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2hkxokphd.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ijvwbmnr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ejcwkaqt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hfiqrzxp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ziutbdah.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2wvwkksmp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ptijjjtj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2toftpfil.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2obuthbez.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ozuuubkh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2fqgprcbo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ubwsgsju.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2dhnmokia.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2mmpgosaw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ezfmklhk.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2qwxzhmls.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2wanmlqrw.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fokjkczl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2slmvvcsv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2vobgcxvg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2gbxlsvir.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2uuzheowy.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2lrpxjdcw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bvqvdzhe.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2pqrdgkoa.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2khdegzax.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2zroctpqq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2rykwakqd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2yuaxxxop.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2bkegvbky.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2tetreusy.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2odnvefuy.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2fodqxdqz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2sheounsl.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2isvydxad.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2imarqvga.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2kfnyvcfg.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2hcxrdsou.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2gapwotfz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ixpvkoje.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2tjisfakg.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2amlpolea.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tqrsvcbm.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2fjgxgerm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2hyvvchxw.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ljdrhgeg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2oqfyepzb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2qlaxrqjf.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2hgvazpex.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qydzlueo.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ukgezjog.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2qityisoc.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2hzoyoajh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ntbnwgrj.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tfgvykvx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2bkomrkef.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2shrqudtx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2zblofqth.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ztymfxbq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pwwsfphd.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wgiikrqq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2iwztuwxs.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2akspfiyn.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2sibzefud.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ddewckwr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2vvqdaiix.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hbfbywkq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2kcscdgtm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2djscwtmm.html


<!-- 参考信息 -->