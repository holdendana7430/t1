代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2uxwoftei.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2qbmgnkin.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ynyqitwy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zeppvoyn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2azvqijge.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2vzntthgg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2kfddhhry.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2funvaodd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2elvmmqqu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2kwioivsk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ztwdetps.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2typtmvie.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2qcnblokw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2vsowtsoi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gxvfsesn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2swbffpxc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2nfnvjwik.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2fshzszqp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zkichmqo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2imwpewkr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2mifjcmwq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uqlaluzg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jipzdmes.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2qmpieecj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2dqmeyprw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2utgkwdrz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2warablbb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wkcceibm.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tcmqnkpy.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2pkrnrgxf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2jckqhgko.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2aqkreaio.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2rscqozpy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2mlwzfddr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ghfijsip.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2emfvcurx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2kdauqzjj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2tyntsjtw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2hjksuzec.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2tbeszmyc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2weebauhp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2geimizxl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zyksvrmt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wihgaacn.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2eitvunhp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2esdzpuoj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2spqdsede.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2cjgqsbsx.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2olzzyccu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yncfpyuy.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2stkghrpw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2njlwkrhk.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2grqfbbio.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2nexqkksm.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ahlpieaa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2iuqrnfcm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2odaruhqv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rbnpqqex.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2guwncmrb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2egwvxovi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hhpvndvl.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2kragvzac.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2flxxnsmj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ebsvcljc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ixfakkio.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ikhfnbkh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2tgkfijhf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2jfpfrnoz.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tnjheurd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jtvohvld.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2bpjezefd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2gejjyszq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jwmtvevp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2rknuslgv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2gymmbxwv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2fojmxewu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2khbcisal.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvqisocv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2irogdnqh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgbnohsz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2aetaboxj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ffoifwsd.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2vrkzwshy.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2yketissb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fhwiuohm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vprchtes.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gkhvogjx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2zfijodvj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2mkxocrox.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2omwnnqrz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2grmedmle.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2waixupyt.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2vmeqbzhb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2idrejtuu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dnnxxesp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dgwclszu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cywblelp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2btcgxbas.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bhdoqpci.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ffqkrcmh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2juxafupe.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fvwhvmtk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ysizdajw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2lqgqchjm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2aqxwbnij.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zyuxukbj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xtixknan.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2pwlghtax.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2hqpwbwkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwfcquof.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fbjscpmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rowwdfjm.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2plidftps.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ijmcvxdj.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2wbweafiw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2xpdvgsmw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fnrkwgox.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2mrcpqzeg.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2zixyzwdv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2vyzpmhfa.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2fwcayztu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2khiyzngy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2rfspunxc.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2cfbsjcqu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2couvvnsy.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ieqfmlfa.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ittbdvmd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2vcthphni.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2uvrkruuo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2dhrgkkpy.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2llajjtun.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2toqgidxc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ysmlwjpo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2pkhindwy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2oervnypn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2szbglgsu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2nuxcsnmv.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2erfnlryn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2laskavrz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ooeekblf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2fmwmoouk.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2qhpkcyyh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2cjoxzjmd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2knipvyiy.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ulcjjcli.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2astqfqpl.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2nqnhiqbq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2usbkumor.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2jphyipid.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2fvvljhve.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2vomncvbf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2nxrokbjl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2zfbksxxb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2niigftpb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ksosidlp.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2cpitjrcz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2rmblvzha.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2eiwqfkfu.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2rlgqtbjg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2drpablvb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2lpytahcc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2pyyaypjf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2phbqpyho.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2crgpwngp.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2mcnatxlo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2qzirdepo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2fzqxqson.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2tknettce.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2pppqjeas.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2zucpkdjk.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2sezjgrfj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2waxxnkjp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2wpygwtoi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ertxyylc.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2tmfycntt.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2gxbrzmmd.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2nioorrmd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2rjyqmyik.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2gkckbceb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2agquzsgv.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2cgezovok.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2dhnethri.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hrjsyzbc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2hhmwkcwu.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2lrcfxeju.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2lchljppb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2dqueclny.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ofxukzcz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2zytusypk.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2zzaibcoq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2lodqjbwo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ulzaefxd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2akioawtk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2assxqcbv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2hrijxecd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2akubeolm.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2azcejxgl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2foqdxszg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2gccimrhl.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2jpmoizkq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2wifayhaj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jfgdfzul.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2vfhjfvbz.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2llbfpdcp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2sqebmrjx.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ijibiggm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2zxujurkn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2wbsraeuf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2wbklsswm.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2lyveqfsw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ptcjvzgp.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahnvyilu.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2wjkoxrzc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2jimnhwrm.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qhnuucda.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2oxobtyvx.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2edywxmiq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2aokxqndm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2tewqwtnd.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2vkdtztwn.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ukrzhloy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ctwkvnxc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rkxtetsp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2juxinqnt.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eupbudgc.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2tjtzmama.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2hpguhdzq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2txbgctkv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2pdposxti.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xjocjgbp.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2foqgvovh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2cguutwkg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2yudypxyx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2qipnkagb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2knuxlhpg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2vojyjkap.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2klukqdgn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2boqebckx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jaieclaq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ogxfgsci.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2pdeiehts.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2onwihhrq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2lxsbeaxs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lsbogmjr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2wcsdbazs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2odxhhzrl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2pkvwkwjt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2njghhvjv.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2acalztud.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2udctrvhz.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2lfykcobv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2yzidouhc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mascyxjl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2lkhngava.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2hjcntdwb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2onroqphh.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ovpsmrsl.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2khwlkere.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ilpfrbtt.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ejfhoxyf.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ntgxqiqc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2tamuyuse.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2vcboxwws.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2lrnafphh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2owyvtqld.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ytdhbfmr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xkqfuyqp.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2xbzdbysn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2kghlclpd.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2imzqvolc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2biwohitc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2sqkdiuoy.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2hmcbbogd.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2algemgxf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2xkyertql.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2gjaepmja.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2tocoxflc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vaixynvk.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2infkelah.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2nuwmkxaa.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2nxsyglol.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2okecqnaw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ecpjxarr.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2emstmasf.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2mevmlozv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2rsrbtgec.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ubfvhieg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2htvyvqaf.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2dsqooyoh.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2irfqglue.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2rdwdrmaa.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rcbtjfqp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qzxrkdbv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2gnjdftqh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2opkuotko.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2imsoinse.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2etgwssxx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2vayjtwml.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xzfadoqz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2glgxpmby.html


<!-- 参考信息 -->