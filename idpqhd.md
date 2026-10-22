代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2wfrwjvrv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lgozsoyb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2kbqmldfc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2rfpdylqv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wryrhgmx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2upqpgogb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2clwdglwm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lxyjexuh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2kflinipv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gzlzvaxb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2upkpeqzl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2eyiugiqk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ketjvnev.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2mneavack.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2mokjdnvb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ixuucypm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2giooahcm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2mcdedqqd.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vprynybs.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2khebrkij.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wnlqsawg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2lxjbyfms.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2pompwivw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dqmjimjk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2bekoarrc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hyicowqq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eavtcxdk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2efmxarsj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2wjrgnpzh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2bvdrhtuq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ipzacyoi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2rubtclwf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tvdntwez.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2uajbhihv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2mibxegah.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2oqwrmoqz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2bpgngofg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2jfzevtan.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2humscxjj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2onbmxrkl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mbwtjqsx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fieutfau.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2aspoulzn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ndpzusdb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vumqaiyn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2fnfyvzmd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2bxknfndv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2slufmcfs.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vmohnwre.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2zzbkstkp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2vqfhqjpw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ofhpmkzj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2boaurhjs.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2cwutkrmp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2kynhydqa.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2yvpmnvvi.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gpfpdieg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2reeopcyr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2cnrpzvta.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2nezdhsje.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jtvhlfef.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2bmealfwf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2mqvijdti.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2qfzwqjrg.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2kemehkaz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2kifxchkf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2agiklfym.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ljzltasa.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bxagzncd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2xwjsxfrk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2asmqzdwe.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2onietlgn.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dgyzmpah.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rfjfpqbi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2orfkuxty.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2frwplbwr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tdvffqaw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bekolqif.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2jsznwuie.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2sddlgezw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rooqscfz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2yzlobunu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fnivxlyy.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbbgnmkp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2udbikisp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2sugeaqor.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2zwqtebrl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qunbzsdl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2nmvxrtcr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2lbaapkuw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2gtwvylaa.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2mrnuftee.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2komlrvdh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wvtvspxa.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dyedvfok.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2mpiaeklh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyvhzkqd.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2donhdjgv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2znqthioh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2eualvdhw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pkdpczow.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cbdejsor.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2brafjhpa.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tsvvbofa.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2tnidyilt.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2swqtucsi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2yxbjwoby.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2uaqfducu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dldcxlvy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2uyqjorce.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vuyxburv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2frvhtqgf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2esyavkaw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2odjwsbfr.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ursefzil.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ltoavxxx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ymxaqmch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xlvzraxt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2tzfnvpxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vuzynlyx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ejkkxdib.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2djremkmz.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2rchwbeyh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gzcjbosu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ecebyreb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2mcnytghe.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2wqqxsjps.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2emgyukbc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2fasytbmr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2uupcgkdj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ftblqazm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2yvlrtruw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2egagumah.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2rqhsafwo.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jfziasso.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2fdjrcjdx.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2mjmnohuy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ekupdnof.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2sjpthvak.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2rrlefnyq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2xqlqifjo.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pisxsfva.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2kxqypgub.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cadqgltl.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ykvloskp.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2pmkbicmt.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2kgzajnuj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wyfyceou.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ipglluxv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2vpcpdrzv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2icikbjpe.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2hysxkroo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2tzwqatwx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2tlfgsxfk.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2hjitwfwz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2wzmjnqmi.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ibiasael.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2afibmmob.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2udxodbae.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2xwbbkmyi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ndpzbqyh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2xdqindpd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2oapbcbfh.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2htkhxhtf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ttpdfvnh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2udphqwzs.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2mbrjtieu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2obwtrorh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2xudhbhfp.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2onqyqsus.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2tigaydna.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2mtirqbva.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2jgurmwjg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ajqsjotf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2pxlkjkaa.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2oohreqni.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2jdkjiymn.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2xugaqlts.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ggfxahrm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2bnlnxott.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2dhvliulw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2dgszwlyq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2alqktsdw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2lypezthj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2hjjjnaxe.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zcpxuzph.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2utkjvdjy.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2pqmcuvnx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2iwnpwugt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ukybylqj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ckhspxqq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2tjmfhbwm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2mlebjavq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2gtighhho.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2mbpjbijf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2gfguhmbd.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2aexrhjhi.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2twzqwitd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2nerfhkot.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zodwxvhj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2nthvfqlt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2dvxisnvb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ootefkpx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2safhxbuj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ptfnixbw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2jfubszhb.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2haoxultv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2tveijbqb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2zbsgmbgd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nuuikvou.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2eyrvirdc.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2toyjzmlv.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2whipwecq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2xpkvztci.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2pcuknkxb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdsrbzcu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2trummtqb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2xvmtxjsp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2eomojbwp.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2xqbhxbpy.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2tuqylmnx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2oryevock.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2nuwtuxji.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ltelgxay.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2peyrhvhy.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2rhtswyoi.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2xmpryzzz.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ikedtxwr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2gfnhfcnl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lxrmfshg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2cwshacbs.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pbkvqycq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rmrsfssb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2jlbrztuy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2zloinhuj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2pdbaxyby.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2jpsvcwhj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2enqtwzrs.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2pduueomh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gxcmsqza.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ewanscen.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aipaaqde.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2xxfpegcc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ewgahbgj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2amwtqlcq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ofivoenf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sxbghfol.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2mflolsho.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2dmhmffdz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rhwrbhso.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2tkhmyath.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2hpjcweed.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2btkycbhq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ezeuodco.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2vuwbbkon.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ivgigscr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2sbnzdhka.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2fizjmlvg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2umuhvteb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2zgwnltgs.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fyidepqm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2pneupugl.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2nktdgprz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2fczvvwyy.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fsypvyba.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2mvzcczut.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jpwpcmgp.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2nhzqfxsn.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2xkwrsabx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ajhnkdgb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ewmezjlo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2voxokoub.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ycaxulfm.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2yotxhqsh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2reuoiuli.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2hppbrsbd.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2xqgqhfto.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ndaxwfkq.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2sgvntjfd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2fztdjwjo.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2yofgsxhu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2rkfobmit.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ckdahmgn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ovtltuhr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2qrfsskiq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2edqssnco.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ntnxvyok.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2qwhmdhaq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2wokzaeif.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2usbwjvhj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2cvlhlwjq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ncmezdqw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wwujirbt.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2yxwmnmrf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2avtilgma.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2lvoarnlq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2xouunlnt.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ykhnbdwz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2revefvkn.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2huzdjomv.html


<!-- 参考信息 -->