代发 wailian999

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3aobkakhj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3pdherpnc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xbgisdjp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3pwqklkhe.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3cnmhflgr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3oxjfpeyp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3woccesrn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oupmvvyl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3chvfzosc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3llaeumso.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3oljsulna.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rlhrikpn.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3qoirxocj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3opbjkibb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gxjvriab.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vzvjopgb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ogsohvia.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3txjmrjpr.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hnirvraj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3rzfplwse.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vcgozqqy.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hxzgghjc.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3umqgvoci.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3mdvcasdl.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3pmxiatpz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3qcjkmiju.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3zvijodmv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3affskpbw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cvrnpkey.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3dghyudgk.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3bkgcukzg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tgacyuyu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3xocafatn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3wwupeolg.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3nmfmtsge.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3abntdfgw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3zyaqmyou.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3kdskyird.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3uzupnuaq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3birvwfal.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3etynknnd.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3vfwqjagp.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3hwwjyujy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vgartmpp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ttkackuq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vygtllch.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3takncqvb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3txysdozm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3njtwojtv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3tsgltogu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hceiaatz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ttnjbiwk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vcucptsr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mbhklarw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3lyfncxrs.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3jxdonolr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3krhfksqb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3sikhbwsh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3loftkngj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3wirboxdj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fwasuhnf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3xvnvtple.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ortjnlcs.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ftwacwtj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3adwuieze.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xmomnkrn.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3cdgavotx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dsmcyrhl.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3budgouba.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3jmqjuryj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zbdcwsuh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3urdqyzyg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3pscqknxm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3rwnnxqxc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3wyprbbov.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3rvtydgdl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3grsbttep.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3dlneqhpz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3roykomri.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3yqoiimtv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ddhkyuxs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mndhcwfp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lkardfno.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3fpdjqoya.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3xonfwhxp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wwscwzxs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zwabohfm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3iplgphrw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3tiktdblh.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ylltvdiz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lcclhmmd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qjjcekvc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jbxnxwtg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vedpqdkz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aosfawil.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3bgfxlrmc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mibzfnwr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wdhbsyqu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3sablkcte.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3acrxlrsg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3bkoxffze.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3xdbpkpbq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fxyncygc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3mtuzonnz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3wnmuxnkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcijlikf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hqgsmcke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fobadhnc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3rzalqmkq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3knmtzvpo.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3tyqfjumd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3hufnxsck.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3zgkxugyt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3cfsxpfvn.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3trbkfxoi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3qshiqrya.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3dquzlfof.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3czfsenzr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3mesxldoj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3spdeozgu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3vcyugagm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3jjntepox.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3lujvrxfq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3tjacorpc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3yndeppeg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ydjuxkft.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ozvwronq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3uaucmhap.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3otmjlcga.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3rglkrtpf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3iitnkurv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oupbwfco.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3imozzhkk.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3axpmpndi.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3mkfhsnag.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3shijwtra.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3xpuhjcuu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3jtfwweya.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3itrpfwvb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3dizyhmkq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3fskuilaq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ssfkfcwe.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3abeblkjq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3yeqrxara.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xuihvpkn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gohchfij.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3qfqhwfsw.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3zalqjdlq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3kfwbxyak.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3eugzmxot.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3pzfpvjyz.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3oosgiazb.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3mjzsabob.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zviolitn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3cyoypizz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cdlmiebi.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3gqqnxipb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3edmooaqn.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3pszqkazh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3qryrjpji.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3euesdboe.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3uwpnwhvl.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3zjbsmkya.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3icpjpugd.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3riyybxxi.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3qwldhohc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3pgjsdole.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ppswqyzl.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3geitejwf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3fzsvpawt.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lbskrlfg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3fypbcxsp.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3cibcxniq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3cfhdfksl.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ovlqqtep.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3thhnhsmq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ekvgqljn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3jjgpwpgz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ugutfhrd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3yxmlqyfd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3gvvfmudm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3kpmekwou.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3thmojdvp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3vmxggudx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3jmripuam.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ndokfapa.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3lshgobuu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3twaravmf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3yagzzifd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3lvqcfvrg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fvwgicvf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3mmfwyexd.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ndmlxdze.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3yfzjjttf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3fucmhpga.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3kswjhihd.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ljsloacs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uujaeceh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3fxhfqzyw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3iuyhnnrl.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3gcqzzank.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3onvpcwno.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ubkuarse.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3efrjhffl.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3frmzrxbs.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3skhfauiw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3dninhryu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3suhyjfml.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3xffxfshs.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3srqejuvr.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fdfaosoq.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tpqldlpr.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3bmehwrkd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3jiscpibv.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ehbdrhou.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3sofrxulj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uljaedfe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3vnededtc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3muijhomc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rpcjexbt.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uzbdxjrs.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3urcpzzme.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3blhpcyzf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wwthcsuf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3degduhqz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ynwfhoud.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3jdjwmgxf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3hfkhfhug.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3eibwdxzg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3cqpkrptk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3hictdjjj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3yeuzzult.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3zttpfelf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3mnrseshz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3doqtohkq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3gxciailt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3tmoqrqbm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tazdpcdf.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3gkmrithh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xuyzuysu.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3upfpqtaa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3nxdjfrwy.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3fvnkifie.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3mjxumlql.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3uakgptqv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3pbxauypw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3seiyourw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3jflqkcub.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3fhackvom.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dhjdpxng.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3fkxockby.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3evbeeqkv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3dgqywxsp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3bsewbpms.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dsjfewdl.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3euhponud.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3btsemcec.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3hulndkka.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ikqyawed.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3wwcggemq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3qypxhbzq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3nzxjciyc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jnydmvlw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3jsvyuazd.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3eptrrlli.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ntsbhpcb.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3stzygbnz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3rudojvuv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3tvxuctxm.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3sfdwmmpz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3kmmroisl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3pqrmovxw.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3slyptaqz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hvdybgzo.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3yzhqbrti.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3vogzzdyt.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3zavtddvv.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3qixcsmen.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3tczozrpc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3lsllcdbk.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3vwwgyxcn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3jkejjaey.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3cfoxxqmz.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3uixpaako.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3sancybps.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3skobyfdm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3jpnoumdw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ofuhsjlu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3lchmofal.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3qqubsndr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3clsebwgb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zybpspdg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jtfxskci.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3sfjuwgpd.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xqhgudhz.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3avgaabnq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ezhxbozg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3lxqwtynm.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3bwbngsxx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tdnazuns.html


<!-- 参考信息 -->