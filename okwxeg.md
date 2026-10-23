代发 wailian999

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3upzwrqdh.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3cjjtdkid.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3jwykbxfd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3nkjdpslh.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vzplhiut.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3wxoakmnr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3oditzzaz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jwgtrhws.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3sveilpnz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3mvbnngdr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3otnfwiqg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wlucmxhq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3lbcdajzb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3orquwjiu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sxoxklao.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3suabhnsn.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3qvdfoccn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ehrwagyu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xavxqogx.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3vvytaovn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cgeotoxo.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3aqishkoi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3jkechgdx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3iisubqzd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wtjiueur.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3fypmmwmr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ubugmeki.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3yuswwcgt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3zhyzajun.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3osqkyllg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3nlcltbhe.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lbgjbman.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3sqmcfmng.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3whivntgv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3yqwubxsx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3tscphdkr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ckinbkkx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3riucumve.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3hyumyuqg.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3bvqfhhdi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nqiixzkf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ucwlitkl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ygkxirha.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qweedwgi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mlxrnfcf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uepygpas.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mxxrqjif.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3fwhmkkyw.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qlfpyqzy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3jswmgsqb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hvksoyze.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3edritpth.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3kuiydryr.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3hcrzhpxx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3awmwnfoq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3bsbbluzn.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jqpxzckq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3lietkhxe.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3lsgpujib.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3lxpspsvz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qeyltuwc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3gwohdqbd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3uzvueevx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3vnrpjldd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dqelrudg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jgkjowrc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3eykvvtnl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3cjzcmkrt.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uvzxyxhr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3azdocndp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3romyjxxo.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3wvsijqew.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rzxpgyam.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqzkewbe.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3xkwzumdk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3rmxrvjyk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3jlmdnklt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmtsarsf.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3zcrjshqd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3rhzlxate.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3knhcwffm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zoubnhju.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fgkclmzc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3qtthjstt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlwvrhem.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jltperej.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pivkwsfu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jbspomhj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3yxaagwje.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zmsjwzdf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3odqltyjz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3erydriaq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uuczczxr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mejdsoni.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3qhevnwzd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3pyxnadnj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lecvzoue.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nelifjsg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3obcqnpoh.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3iihiluwu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3yvubomgx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3upfvstgj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hmikwirc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3rducmjab.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3pxsgbrqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgorvlqs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3djffmnnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fdtkwxko.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3agsvsmln.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ktsgouvt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ogfpspwa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rjqcdvyq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3cuskvveu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3erexdpdu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3boijoifw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3apeuqftz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3qvmffbtd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fvxouvzt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3yduqlsog.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3pnplekuv.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3rjqiilgp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3jzbwhofu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ojwgbfsf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3epsexclb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3netimzzp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3azhqcfbb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3bvyrccyw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3uggblpjc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3steaufcr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3upemerbv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3kcrseqbl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3upqaaqmk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3jliaqkso.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3rykvcxaj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3cghvjpbg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3pkppczlg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ygxlccff.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3nrnftnlj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3wqrdmqgf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3tkurttzb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3sdyqxdlc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3yfjbqxdx.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3oimuhrzy.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xfcedhqs.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3trfuotvn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3pqmzoblz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ueatjjrx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3culeplhr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3rehxbpdc.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3yfhtvtuc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3turokwev.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3flkuomed.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3fgukmbch.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3hyhvkkmz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3nnazimqw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3njzogctw.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3educwqtv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3qpffhfax.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3gsxpmrkn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3yxokzcjx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3anzkbhkd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3zpmaeqoa.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3juqkhgvd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3mnhmcxat.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3xdyahlvr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3reetjpss.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3etdijmpv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bdfrxatg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3allmkeju.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ojhpshmw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kdwxnape.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3xodkkzdc.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3gmlyuiro.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3wmbfkkwu.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3tlwxmsqz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3cabcsjtd.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3tyaxjnsl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3aepbqoyi.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mwjlcizf.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3epodjobo.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3xcvxkbad.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3mdweflot.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3apurezlx.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3iriuxsjh.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3bgjptefd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3jinzfosz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3qrcvxbcr.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vdesymzc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3gbptdawq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3fadyttql.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3gwzmfegf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3jdpwymlq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3axlreijd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3yqvakvvq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3dvjgppmv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3rcrjyfmr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3srzyyyrn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cbpngrxo.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3omozxcsz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3kxifgxzy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3xnjqibge.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3foogyffh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rjxfmmza.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqnpcdty.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3xmltjscn.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3wmoppglh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3lavipyky.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3zstuyxat.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3hyzvlaca.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ebytzyyy.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3fwywmtze.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cvxqbtxx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3viqhyoxf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3bnqjsxrg.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3dzowazgb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3avaexvya.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yroqmhlh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bbmzipwl.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3zzrovcau.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3frxsmtcr.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pkowegem.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3zdcadmpc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3rqaacazq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3hekowaph.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3rgsyjukf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bkskoxqy.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3kukifkgl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fupscqle.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3jjobhpzz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3evmbgelx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3fnmhaoip.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3vyhwowmm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3nwjlwvlh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3dmsoxule.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eyvobxba.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3cdbwmmcn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3xdcsuiyh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ejivgqyn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3bvlceprg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ehxbmkge.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3vwluenou.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ktpdswys.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3yziyegbn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3tdjadftn.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3swkjazvc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3xkbeenmp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3uycwiwow.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3qpczjtmm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wnlsjtdc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3miawvyuc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3qvnicqmk.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3iwpfgbob.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3atqoykfb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ghitghlc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3oousfkrs.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3zhahcztq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3uteufqnf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3eygkubkv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3wzyfgymu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3zpbvhcrw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3dpeeswhx.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3fdghmtqn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fgoekyhm.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3wjcdwxjk.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3vlqafmbf.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3wygrlkbi.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3gsrzgskc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3upiasejd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3bczekwzb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3uprpimhr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3cmkkccrd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3xtktanfi.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3keprlhja.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nbywtewy.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3lbnrxuqi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3lmxeqrzg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3yxcfncfp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3qiarynmc.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3glrwgunh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3qzrjotzz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3zfherhsk.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3gglknxsn.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3pqgyhpem.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3gzpqvquj.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3rdqhvhql.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lybzomby.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3iwpzsdup.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3popjyubw.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3majjggrg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3pkccdoim.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vtpgfohu.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3yuoxgmts.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3tyhthcpu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3byreadwk.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ctsphkxq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fmmribxl.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3weinusza.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3rptekvih.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3aqkzydsj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ibibghqr.html


<!-- 参考信息 -->