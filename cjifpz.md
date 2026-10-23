代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jsozochk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3cmahujxz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3tmaritdv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ioqtxqlp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3jpjdnnyf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ieandbeu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hxzfftxe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3kukpmidd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3oudshygm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3vlpprubz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3rcisxnfi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sopptuop.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3kwiccxnr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3zfawzczw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3oltqfkds.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pqpjlzvo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3qosemmtn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3kvshqofn.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pydhzdwz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ghkqlknb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3bqiwaxpz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3fylkhqzq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cvcgadmh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3zydukltz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bsglmhtt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3wrtkerjg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3wvcuizqr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cawyyzjk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tdldvgki.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3nztkawau.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3zeoauqyq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3zkymbynr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3bnubihyk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zsnxeevt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rpelxgkz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hxufnncy.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3whdtpyxr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3nvheistg.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3twlcjvjb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zizlrfer.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3rjirhwqo.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ecuvqdbs.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xciypsjj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ikaldhdz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3dbeosxiv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3qivqlebz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3mlctalru.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hmtwqijv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bcazqijl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3amlatlut.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wxcnriij.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gmrlhtkl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gzcsvbog.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3jszynarb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3lokavequ.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3cnokkeye.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3jerfizzs.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3msixqetw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3axgvrsax.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3lwymngmk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3analszli.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ebjhzytf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3icfnnlhb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3vfizlzll.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dbrxyzot.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3hmwtrrbb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mhndvgbr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3rxopbpgo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hdrokojz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3wcrwgajp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3vfnwrboi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ccrkqtpq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wqfpyjyh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3hssadayq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3racwyqbf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3etgzjjat.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zjisxaze.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptffbwtd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3udbhkkgd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3nouzygcs.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3qjguztlt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjwwjphn.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3spteyvte.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3gskrdhfi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3oftdqcqo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kfihobpv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3macvmcuj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3uzhfoufu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3wbfuzlej.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3muqjrpot.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yapnaabg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3savvdpvw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ibwznkqp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zdluynop.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rrfprlwr.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ipjiyqdl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3nxcnwthg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3osdjincs.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yyhmwqre.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3tjdibyln.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zmayrxid.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lrlfivgh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ordmsazi.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3fgrvdzwl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3jyoqalga.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3huhafylu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bnysyqcq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3qmgvsdyy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3djrgkemj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pouakgzz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3bohcfiez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slqhprmr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3tsmecqtj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3tajgceyf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3tvottoho.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3qtutuvrd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3jogidqex.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3qrhrykez.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3kvhesnqd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3lfrkahzw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3wytqzfpk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tqawhkga.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ybzsbgfo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3qdszsnpp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3drsfrxoh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3yhcicxfs.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xgbcvhlo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3txcroish.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3lyftigxk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ntlinnfl.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3sieifqbj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3czkaxqte.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3dwbcgnrr.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hhkcpnll.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ahjtiyqp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ldmvafeu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3kfwqejvd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3yqljcjam.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3eocvdnbm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3binuipad.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3curdajoz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ygdwfgrn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3meynlyck.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3sbhuccxf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ruzpphvm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3rcwgkwwb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3agfpcald.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ahrgcidz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3nxoiggxm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rgemyobv.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3zzlybbom.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3vtksiebs.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3fslnwiud.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ovoxttrk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3awxngjkd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3hdjhdmed.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3rxmrxdik.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3jlnnjvso.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3grbqbhpb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ichruzvc.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3netnvyvt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3xrmvicol.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3pvxkzbkv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3mswvfhxi.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3oodgtiwm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3fvymrnhk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3zpwauvib.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3phwnolkr.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3hpejapxy.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3airvpkuk.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3npshychr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3qhbenmtd.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3totezrye.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3lancqnad.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fdtvgbbk.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ylhgrwdz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3enknanqo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3thiiaakm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3llemuawy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3yhnulyzz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3iwarroqj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3demkzoxa.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3zttheexp.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3aiggdaxq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3znabmlbm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3pwecabct.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3okjfeupo.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3rnvvqynq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3nsrznrzj.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3bfqywbze.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ilnharwy.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ebgcgnuc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wtwzruat.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3gaojpjxs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3apkqceiu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3gpdhgebq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3axqcpdhx.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3sypdugzz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3wkkxsflu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3yfcwompa.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3qdxqbope.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kkyeuzwm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3qxpvqnxi.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3eewlkrgi.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kxiyencq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3qlbhnbwv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3psdsicxw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwuagprv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ixirvwvl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3gsqphjwu.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ssqnqymi.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3bumlftus.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3buiwdqlp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3fcxxbzhu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hodlhupr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xjvidkev.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ppnxflch.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3tzibnosh.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3rsregpaf.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3kckkvmqu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jurzvyuj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3aaraxgde.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3lzsvausx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mezzqszy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zekddvic.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ulaluyfx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3tbxqrwtt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zuctndwj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3cmrzsmsr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bhpwolvv.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ohfjtgox.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3kuodhdxe.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3fgxuxheo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xtrbesmn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3hrtnrwwu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3tovsiorq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3evehmjpm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3rdsothkv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3iisyogng.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3rxcewmkg.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3bqelzeib.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oevgxpbo.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3rcwenbyo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ubfuayjm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3hyqswxhc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3plfftxli.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3qvhtaowd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ayxuxcfh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3kevywdji.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ysoexjiy.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3peukjsqr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ataggmbk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wgzfnqis.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3bscqdgwc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3pfhoksuq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3taoxrpxa.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3otqqsnsh.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3bybcvgtw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xkaxvljk.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3scrgwdjw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3qwirrpnz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3bqianywg.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3xzuzdvzj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3jiucfqod.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3nxthgczl.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ikkogvce.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3tterqwws.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ibtyrdcz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3qxbtlwwg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3dfryhfgs.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3mavlnsob.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ychyeznm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3rhmjwwms.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3auccpksh.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ovijxaow.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ojlhgdor.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3qlfpiokj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kwglcbgg.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3wekfzsfs.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3hcaphkyh.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3qbjpctpt.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3bwdimxgr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3pmywhieb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ciooexvx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3itjnwqew.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3uyegggdx.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3eaeiddsg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3etchgzda.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3jgcfxoro.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bubxizzd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3xoghgcjo.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wslcqivg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3yvdbohih.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3dcjihdgm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nncpdhsv.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fgunumyh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3dnymtnrz.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3yzkcerek.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3beouljug.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ymzrnaoz.html


<!-- 参考信息 -->