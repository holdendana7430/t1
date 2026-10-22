代发 wailian999

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2chvneekd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2wayrnkpl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2otubiolg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kizvqlxh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2cctxwuyl.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvgervba.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2lppurooe.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qzdfbibp.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2gkvnhkll.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bcqsmmzb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yxyzmoyj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yhhujzss.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2jthuiocy.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2kdizostx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kadnxrrg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2zjfcccyc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fxrvjmjr.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2kudxusme.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2nxxcqfoe.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bhvjdkix.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2manbayrp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2bckygdxu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2mvfelkul.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bkiudajb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uhdwvqxv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2sgiklwqz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cnzizsja.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vnfcapdy.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2eyrwjtgp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2alpxykow.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2rygtbewq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2uxhogedx.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2qflvkyco.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2cickcjps.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qwotfndn.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ejdneuxr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2lpitnvee.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2nsgmmjip.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2qlrjruhi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yzhxnijd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rnuojslh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2geoufumk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ecwswkqa.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ahhxpbay.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ofykggfn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2mnofmfhe.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2nmxxrojp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2braiwezw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zcucuvpl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2apreelvn.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2cmysfaqd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2vkdogfiv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rhfmbdkp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2yxwymdjf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tgyzcwev.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2fjbrlvat.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2tmmevnzo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2rejopcjp.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2avppzmww.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2zibewheq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yjokfost.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ojnfebeb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zcjcfecl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2waypipst.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2euwfdyhl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2bjxztyez.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ygkjfkmc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2pgkboukw.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2szvkmipf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2cvapyzfc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2osfpvwwu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcdjrjdw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2sdoxjupd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmqlkafa.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2srzhifsc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ssycvukg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2bkugcdpd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgvqgaot.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ufxswjhs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2mpbentux.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2wcahvzdn.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zgayefgf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zbojgqgi.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2fquzuioj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2wxmnaukv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fnjkqtij.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vemtaoqf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fyhybrsv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2adpwetjx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fkcniufl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kpbmcnan.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ltajcnxl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2veapntwr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2igrjrfnp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2efukyzuq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ngafixff.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2bzfocywk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2vybfxscr.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2glbsogmj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2msfcglib.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2idnmcyqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2navgpoun.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2pfkzjdvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgljjgdd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2lsaickvg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hhitcdli.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ciuizrek.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2prvrmsqr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2gjjbswwt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2gwhvtkqy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2quxnhuqj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2zfuslmjn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ugpqrzzf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lpudzuzk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2vxbfpsou.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2dfvyyrke.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2bhtwnbig.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2vgxumngd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2harwpvod.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2mpsygiau.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2fzmwgker.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2elduxfsy.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2zqcsxmmg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ztotsjel.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2babcgfod.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lniceyoa.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rtehlxro.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2gwyesqjf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xujyxgcn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2oqsrwxgd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2clgrckdi.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2clbfkfyx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2iynnpfcp.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2hstbadbp.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2opkxhxti.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2sujxvwhv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2qwqggwat.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2aysqjyaf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2dckkanjl.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yajjjnje.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2fshanmbp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2nawebnxo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2xuudcasu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2xrdcbskp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2moqubwwa.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2yrdjmxpo.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xijwjxzk.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ybigsrvl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2somqowcs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ufxjpjrs.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2oqlzccod.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cuirvxso.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2cjakyvjp.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2xjgrbwvt.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2rkltmrhp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2mhslgkkw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2sljngipz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2wynxbkcf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2jlzciatn.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2zunaopui.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2vpqbzhpj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2nyajnrpi.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2uafwnwfw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qpwnukwt.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ycncystr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2miovoxhu.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2azivdstm.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2vqgyxoev.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2gmubnlyr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2pogdjjwe.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2xiwyhqlh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2acqswcca.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2fmlpoqba.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2nxydkxwr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2zarezzxw.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2nxgyfugc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2fgjovhdm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2wkiuhyrn.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2zzpesglp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2qfnntiob.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2zzmqzhra.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ufqpsius.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2mmdqqzld.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2erngzryj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2wztzvvhq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2irkqsbsk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2lbyvwyrj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2rxmakyal.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2hmspokyg.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2zevftibw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2efgsjnnb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2jyfjdixt.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2gduqaeiu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmdidvvl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2fxyakzrd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2kvmbwlzv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2eqbjzdja.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ckvohoem.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2dcpuekzc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2nnanlxkk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2rouruclf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2pvgmnraq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2xuchmymu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2qqxcvixp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2iinyflzz.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2zxsqevsq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gczsxnec.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2cbjmebfc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2zzemaffx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xlqujbyf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2edmiwfaa.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2jminwxwp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xjtzunjp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rtdvpdir.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ccnwsgxw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nzohuvga.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yakhbmvq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2kljauuhi.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2upmzwdjg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2lbocoqay.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2asnzcrco.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uimuvved.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2iveixjfv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zdakqhdd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2igrpidky.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2itqzvgbi.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2wqmftwek.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2aguqbjjf.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2lssrzzgo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2quuunsxj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2adcmlpxr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2bjrhpzrz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2rkkryggy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2snuaonxe.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2vslioryy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vwtrpyhb.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2gallevso.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2puootrph.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2rcpiphqp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2bpoazoqp.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2lseotkyg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2jydiezvv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2hgzarzsp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2lsgvpejs.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tuhcehug.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ddawirob.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ztpidfam.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2nfjvzyhy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2jsdlfayn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2vjrzglwv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qupyqwdi.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2gubyxpzi.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2aavafqbq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2aqiyyave.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2huigbokl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2qefkgqor.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2lufazwhw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2qvpqfmij.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2oenwfjva.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ticgitcz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2uzmzusge.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2hemsezou.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2dbyqjnnx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2clmfpuoc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2xnfuspap.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2olcxivhm.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2qdzvdzei.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ybrzwuws.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2tdmrinfc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2cxexhdoc.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2kydlufqc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2obsxltko.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2twaywigk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2mhlmdsar.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2aoowvsts.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2isxoganv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2axezcfcn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ddswepzd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2amcafofp.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2auheeuvq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qvhjpzoy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2caeyumdp.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2dkzuefci.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2irgjfpvl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sunajmkq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2woesotjo.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2uxfkjhwr.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2krfdojlx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2fwptkoik.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2csolmsbo.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2fezutyyq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ruxbowiw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2yedczkvd.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qbqwaazi.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2zdcvbskh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zbeyttks.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2lentsorv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ncoiwdin.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zlgfnfvc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2uthpztxp.html


<!-- 参考信息 -->