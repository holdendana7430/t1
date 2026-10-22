代发 wailian999

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2etchzoxt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2xmctwuxx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hldycsbb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2njefwoal.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2xwioouew.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jyoqrkpt.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ilcovwed.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fxkiaatf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mrsahrcm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2kcnzbajh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2qymkvoyr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qtoxfybc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2hkbfzqwz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2tpzkaugt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hiqezist.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zeoqbwcm.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2cpwmxnjo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gjrafpbv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qjddrvpk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2vgevdjmy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fnkbizcz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2tyhavsnl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2oeagyohv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ioxhwjoq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rwlltvls.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2tofqgvzs.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ngzmlfht.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nnpvduen.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2bqdyknen.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2nsmashnn.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2pqriqmez.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zdzxkdgj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2dsqhmssr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2zqfxrvuw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2hpiqirdf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2kczfjhbu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2xvoeovay.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2afubtupx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2cozeikwu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2sndnaghj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ydcgfwkg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nvzmgsql.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ahkfdkuh.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2pvrwogql.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jvdbgtgx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tpaoybip.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ywcfkbei.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2haarnxsq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rcogmkzf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2bzfhmgoi.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2aqbcugyp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2alrqrbye.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2dwnimdpx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2jxtryfkq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2proxajtm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2wlxzgets.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hzlytqrg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2psdrvrsc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2uifejbei.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2dynbzdzj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nqrlwyec.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2kcxgboxs.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2pjmpiorb.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2umnmevab.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zpfpkwpd.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2cahmcwkk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2dfnafawn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2tyhyxqug.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mvtvrpnn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2qkpfzsys.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lznyxbzk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zflzhoyb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2embwgxtp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ixcdvtsg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ycnrlcnq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufxzpham.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2rjydiohi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2efyzewea.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2salhzvin.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2lggzbppv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2uuyflykx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovmibyju.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2imcloluw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ybznyren.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2buqbferk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nagfuzju.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tagzyjfj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jiyxyuhl.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ddgcqthe.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2aehhjfat.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2izgltwgi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wohfkmin.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ndjefifj.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mfuczdfa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tchivfka.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2fggicwby.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tifncvpk.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mfbqdlpt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ioxyxjal.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2rdkpmoqy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ysztmoyl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2xcjthqcp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lqvsvjjz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2aiazpaov.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2jluvarck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tajzwwfe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zmxkilzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osuyhvgz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2zdbajfsg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2occwqjca.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2gjvnpqyu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2nvyxmzbs.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2azbpdkfj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2thhqahfj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2advxbemx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2jzqprujd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2awocvhvu.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2omcnwgqm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2bhxutotb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2rmbhgtmj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2nmcbbsqr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ranfoplu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2neoiilmb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2zdfqmuvc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2rrrrnecf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2rtggwzva.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2pojuxzyx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2xbesnxnl.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2okxqvcsv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ccaxvsli.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ussxmqhg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2jmmbfeul.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2bzyrxrkz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2yztdxukc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ixjpwuzt.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2czprjfiq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2wzchmixy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2jcxcpzqf.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2nttaroub.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2etefxzwt.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2qfxwsolz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2swmdhyyk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2anpawjxs.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ajsxyhcq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2hdmyrkyc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2wbryukmm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2onksevyb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2wqcuqhmp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2vrxqjuep.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2raqbixed.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2yjlxgjnt.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2syfdxxfv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2uunqgcfc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2yzevsvjd.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ovpiktxa.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ahwzcmri.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2jhkjpdcn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2acudyggu.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2jzlvthiv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2zndakvgj.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2obihokqy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2cmnkploy.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2onesckpg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2mwaluhhu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2geeqlzqw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2hosainzp.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zkwuzhta.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2wdokmxkj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2abhfotar.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2pneydath.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2csqtwluv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2glhywbya.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ufixeigl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ksjwdggk.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2bieayztw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2hqhobmaa.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2icejnwfu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2lvbcpymz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ucxegdwx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2yzzticyu.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2arljstrb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2kpzfkkma.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2tprggeqk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2nuavwebx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2yrgluybf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2xjvdmzai.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2kdsbuepd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hdbkdexc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2emtjdgbp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2xxzyxwbc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2qmwmhxxw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2eipffdrk.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2tezlrmmx.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2lprldogm.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2qwoszvsc.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2acpgzhxt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ohzfhoxk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bstlkvml.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2gshtladf.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2quwcltuw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2bulkhrwn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2swinzbbs.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2pbxtrbuf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2naaealca.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2adonzgar.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2acgeqwgc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2obcfyguj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ustswlra.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2udjndjvn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ryusrpbp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2hphuplfu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qtmkdqka.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2isuldbll.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2hxtogdcb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2hlvvcwzx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ocapjjkq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2prjjhbog.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2figpyqpy.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2thumdhql.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2inehjeqb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2swglmmgh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ixwbpddk.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2xlnstxly.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2jgeqehbx.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2zapmonrz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dedippom.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2adewxywp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2yvixewkb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2sygluxhv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2bnafsywf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2cimbezfq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2aiabgqmk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ljyssxxc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2qvdzbocv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2bzaczmew.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ungwptxf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2qxoqmvpq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vhdthnqq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2sagzwiqh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2bsvqknfy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2evncidwm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2wqnffkwx.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2eijuhmjt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2gcqjxwfp.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2kdyauwju.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2cgxqacwx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2tktpjvbi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2jbhvwshf.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jpkyeoos.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2kddofhpi.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2umqnrzyv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2tqwgasba.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2pmfeipix.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2wsugisbl.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2srdmltdr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2vmfcgcso.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2katyrsnt.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2tviimeyd.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2svitfdmt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2fcdfpltn.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zrwjoesi.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2hjbxqrax.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vszgkpqk.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ckfipvuj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ubslujac.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2sseirqhh.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2yhevmfiy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2oyeehljq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ssvahzbd.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2wqxtlymm.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2yecrclow.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2pggkwvob.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2wmwimuuw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xdlmoobu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mcitaysr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2pntuvros.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2xtovmdgr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2vfjshqjp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2vgwwmkjs.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2mncgakaa.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2jfpoxpbr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2iukybsff.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ertmvlml.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2vqlhnmly.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2lanxdhix.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2frsuiwbs.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2klvywodt.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ltrxvcev.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2jbssmidb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ccievypl.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zwvnojka.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2eulujjaf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2csjbxjbx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2xhwjrfri.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2nklkricc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2whhgcsdm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2rayeekee.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2khcxrogs.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2dgfnjxnh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kwvkrmvr.html


<!-- 参考信息 -->