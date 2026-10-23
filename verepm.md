代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jlcgtyzb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3zddfzzcb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3thzmfuak.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ulmsqezr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3vvczjeoa.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3fqgiarro.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3cscnwjln.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ngvvuygo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wzahoumq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3igccizuy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vrcszljp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3erfcatom.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3azuzfukd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3whtzdgnk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3jebdsams.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gfbraopd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jvzmgtqw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zloaverg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3etvvovkx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3btaxbnzb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3cemvsolg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3qnbwnqbl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qvvmfcha.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ixligxik.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3umycqyjg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3rhceotpd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3rkmykffp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3oakaxnvp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3mcviwcng.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ctzndwxx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3aytkwhyd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3sukvyfvj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wyeuodic.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3rybihaxb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3tpgpjhhh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vvgjsibk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gskhligv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3nnlzrwyp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3patcbbrd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wsqxvgyj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3zsnoexgi.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3gpsgidls.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ljvscdyk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ctfhihcn.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3eynftmll.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nnsekwiw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3cwxdtwte.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3fqjyrtaf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lnbrqwai.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3evdeaxjm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rnrhlcul.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xcjyoxjr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lhwlxasj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3vtzxgwqs.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3slwwiqvg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3wnwtmqvo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3arqalqlz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3godvyyls.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nwqfxahv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3eynfnxhk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qvhdczjp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3uqlkokbc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hgetalwo.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jmagwwod.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xvvnaiok.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3yioeglig.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3heffqsza.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3dcfamuma.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3edevycsg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3phkfhabu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3pvvxmwja.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3xnfpcycg.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3likgxhwr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3lkjjugkl.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3dqttdrhz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsnrlfuu.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3fxcukbjq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3oscikfff.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ykhtgoff.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrnulcvj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ctlxhyip.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eaholvfb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3gbstrfmz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3iesdrnlq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yzldyaov.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjknvwrs.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lqiqrcil.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3odmpdgzw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3tiqackcr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ulhvxlkt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fkwqankm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vewalcgs.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ezextdoj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3amnnsnxv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vqffehrd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qxifkinz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3cssgzveg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uwfyeisx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bpiioktb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3xblpmnhw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xllwmjjl.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ifohonsa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yxbqohbf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3lpgvalki.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3fmgjcoca.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3rjyzngeh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kqsdhvxe.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3zpgbsazs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ybxufvtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pcnqznse.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cnbqaniy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvdqrjcn.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3kbfogvox.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3zytpqepu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3qubtrbio.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3noefqekt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mqetpbui.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3nzdtyuty.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3hmqykucm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3kouvhtnt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3svmojbot.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sbgsybjj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3xiilynre.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3wtncabcl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3gsreexpj.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3fenvajki.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3paqvyidb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ixidcjgy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3adkqwlnk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3vodmnexu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3eawvvxil.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3afmhrbpb.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3mjzjwxcl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3cxvduokj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3vtuojpsr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3upwegjbz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ebszumtr.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3jhxxnbay.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3gizptxsk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3vpozbiok.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3vvchabek.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3xdfadbsq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3twqtbiif.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3wwecabqo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3kwrsgvrm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ozeoclbl.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3sqeqxawu.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3khlopzjm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3cqxqyiaj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ojqvqxeg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3lufasiyb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3qndnizrv.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3nzrddorj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3marmzobt.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ajecmlgo.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ibggzedt.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3azaoqgzu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ypjjzvxp.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3gvcpmbls.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rwntrolv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3pabqumdc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3uhbfbskg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3padoousb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3pluftqla.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3vhavkwcs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ityubvgr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3cmirtpch.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3nmipbwuy.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3fodhvebf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3fmicvnmh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3gkrozqdj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3rrsttade.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3gnszsgzc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3iblbyjrg.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3fdgomefq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3bfbijiqs.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3yhvwahfi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3rgcnhkxy.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3dmdzxrlr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3getvoupv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3grbdayaa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ibtnczve.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3sxoqwckm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3pjkfbdyj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3bbvkjtak.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3miopbyzv.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3owrrndzc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3thaolzpj.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3joupmccs.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3geguvqoa.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3atwtjbtg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3irjudbfo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3mmcpeqvp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3avefmoif.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3veanckwr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3otffzfoe.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3qoswqsqw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3surzkflt.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3bbwlchpt.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3zjjmacmk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3fbizlvfd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gyljnxxn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3aqkdawqd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3cofsmwvm.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3tsuzjllj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3vuhvevdd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3evhdutad.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahpzfxyi.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3fqpkuqru.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3jjznzxod.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3zcsdnyre.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbukcqqf.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3kazpxlen.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3gmskyjwc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3aroshmcr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kadkvxeh.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3fvlhdtji.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3twxfhrsj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3vpezngyu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3xowwglzg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3rmnlhkyr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3djjzqhrc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nfdyxzqj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yjjycpdn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hvfcrlql.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3jstbkzrk.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3lxmuqgxe.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3vkorgqlt.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3wldbvpkz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3iiahdjmf.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ixgbfvuv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3fdmamnbq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3npqusfyp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uektsdhh.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3foyujcnt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3wajtjbbs.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3vbbhbree.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mnkqjdel.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zpuscuzc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3rwpghumn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3zwlyahsq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3axkepjvm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3cnqzowli.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3yfgihgug.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3sqhekacx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3csvvmuqo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ypemmjxi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3gluxmvzo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3woqzygqw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3awijkrwf.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3balbldpy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3xoktiukz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zgugrxfm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3wpslyzaj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3etkfbhuh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ucnxhktr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3xdedpmrb.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ezygogur.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ijpchvsf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ugiqqbrl.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3cviglhmm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3wmdxhkgt.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ixnrnakw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3dxmvgckw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3wpcmouay.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3yjptxayx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jocttjng.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3erlbvoin.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3nvtelvqu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3fsangaye.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3kckmuprp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3gamcygab.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3dmaxmrzf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ufdznuuy.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3kcrvplpx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3kdxjtkmc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3mxzthokl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qoidijij.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3haotolcc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3bwbxuodo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3muzuptcr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3rswhqhpu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3wrrcqryn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3gsijytpn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ewivckuh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3lqgvpvjx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3dvmzslxy.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3jzxryibx.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3evwbctri.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cukbsnfg.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3gldomowy.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xxdohxin.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3aulzfvik.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3slzclmic.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3gdxiqcni.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3dnaalfqu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nulymlsa.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3bsgilfra.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3koufbkuv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3hidercqr.html


<!-- 参考信息 -->