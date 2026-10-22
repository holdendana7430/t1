代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jykksqky.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2thxpiqaf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2hacowzll.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ghguefwd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2grarkjhv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ojbeaxyc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2keoouuqt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ajwahjfi.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yjsmoiek.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2wpuhhbso.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lmmvziiw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wkjmtyrk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2srtrpomu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2vwjoswaw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2mxfuxrwr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2znmnktbp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2bwmqllhd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2zzvgcgct.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2gummhkud.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2gmdcwfly.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2tkulpdgx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2yqccpiil.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2gbkqaboa.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pniyxmtz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qoovluhk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2fgvdtrtv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2irgammjz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jjtmfnuu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ygvntahu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2xrphrcmy.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rstfqidz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jiedgdwn.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2mxpmgtym.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2vowrbfnx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2btftvjae.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2sysugefk.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2pdrxnsyg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2piuppoiq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2hndarfss.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2tdpnkahf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jvbjckpp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2agzwshxc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2dhkyikjs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2bozncnar.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2qjtnpkou.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2krvdxooh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cedvxbsh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2raynjiil.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2fpshbeeb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2rfjjdkyn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ydsqgyus.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2obfkxtai.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2kodfwnud.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ahpozdcp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ivcgmcrq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2rltlggmr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ebqnfqdl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gvbdypqm.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2gzsyrmso.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dbpzlrlj.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ghxagjeb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lxbiozlr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2tfdvamhu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2fzucelsh.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dcwxktii.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rctlyygx.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2irnktlja.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2bfkefren.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2hyusxtfu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yhibzaqg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2wlofknpt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2fhmoxswm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2letqnjsr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pfxfqoen.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2clkbilqm.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2zfpnvtlk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rbcxeixj.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2iczishvs.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2mqyjtysl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2pydjmxmg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2krqsefdi.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qxpvfrvr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2rvtzlzuw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2khlinufy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sctfajbq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2uctkbnwa.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2cxmbnnez.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ptthisuv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mowtsnfy.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2blffwvib.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2qvjmznzr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwvfyijn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2cpgjkeui.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2evvrwclk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2hgquxgel.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2pnigotms.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ezmnwolw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tieqirre.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2clbevptp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2lxzsggbg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2oztbxyvx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yuaereij.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2msjkafji.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cwpyfapl.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2wkwdqqyf.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vstgempg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2apjcsnbh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mnewnbab.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2cxfqcphp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ojukgehi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rfgczuud.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2udvyfruh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2pkrpzcum.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zgitvbjs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tmomaqni.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2kkjrcgvx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ufolsocr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2kyzbfbpd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hqeetrdh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2wyqwdiys.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2xqiucbot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yoncjudd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2asxpajkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwgrzeoy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2kdhorwvz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2wrqnprdg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2jwclzvjh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2tpeayojs.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2mzlhcpyq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2dnnvrdys.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2vhsjnnup.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2phrwngdw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2lpcvxzyb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lidwpipv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2mylqptay.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2oamdfpok.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2bpesfjhg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2wjsknkqu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2poabrwgz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2mvrygbni.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2nevybmxd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2vvztdolr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2nnakrort.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2usdzwlmv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2rwoktzwq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wqgxykht.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ctbxjgkv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lwrnogim.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2vjcdwwvy.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2zyhznxjs.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2chpyhyew.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2uyautqne.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2klbyxrst.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2wneqkwil.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2zfoobctx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2cwmyftoq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ebzcnrex.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ppdazpbs.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2kyhukokk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dffzynly.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2vdcqwjun.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2lathytim.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2wxbbjebx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2nvykkpbw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2vgvzpyrq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2bnulslsj.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2witrxioe.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2jwireipd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2nchtlxgt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2qaftnyhc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2mpeeuuqd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tswgctoa.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2qjjfomvx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2hjnpwdfg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2hckulwxf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2mxwaezsg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2egzzordh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2oglarkpl.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2tswoxrtq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2gthpkcnq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2xbzwnfyj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ogkmvoer.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2cwtzmtwq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qzmaldtg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2bhvxlhbe.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wuddzyuv.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2etixoxxf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2lcmcfcyh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2kukdjmya.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2hlyylqtf.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2gpvcdkpf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2qlpzhmow.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2xlpqyldy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2qycilhgc.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qfnjvnnr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2bzrqieog.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2yqdaphcb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2tifgqmfg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2makxetft.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2kasnpfqs.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2nmrmgqzf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2sjqugatz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2lxoxurcq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2cwpjtevm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ibchoknc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2jieqtvub.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2lvdkpwli.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2blagnkvc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2xxtcazje.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2flaifele.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2zfedyajo.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2xfwtzbpb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2cpqcavft.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wkbswoym.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2zwxezefn.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2eiqlwrkh.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2okrzaqeg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2sxggyhli.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2cepniufc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2wgnemfvo.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2wvaqwslp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2jgsginar.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2euriadlr.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2fvqppkyf.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2euoywsav.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2zfnojqek.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2yaczxfjm.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nkfyajqi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2unziqepy.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2yhqbaqsv.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2gswpqdnu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2hkionhys.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2hwuzowka.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2bgenakws.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2yborhbkn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2herpwaml.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2istvjxoc.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2wmgicoik.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ljeanhjm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xhvuavkb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2ckodedwr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qvsvpdcb.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ekezqxiq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2akmlecpk.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2wmbpzrie.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2tuijidrs.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2iearcdyz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2eafbltlq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ljcaeypz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2vhhfrmrq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2zizglxlm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2wtwzrpqg.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2vmlceibs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qyteunpb.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2knhmbwhg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ikopiigf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2kzczmqqr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ssksdwpl.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2inndrwmb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ectvyaar.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ockgjntd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2pywoxiov.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2dvsohbxk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2lqlppxqb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jjlwvape.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2pkdcgxln.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2zieioeas.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2lhyqorql.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2excatngx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2bjxhldte.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kkqmfxtc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2szcjfgsp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2pnumfput.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2djuqkkaw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2uvogveze.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ofwdbuej.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2szcxhsdc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2qgjjapmc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hrvmsvtz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2rfzswlaa.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2neyhcazf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2bwzhbtby.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2bynwgymf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2vnfedhbi.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2kyexqfut.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2astkwplj.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ntgrrevk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2efmfikgx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2bupzjbfm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2csqvyqhg.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2fpqzebdg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2zdplbvnr.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2bdcegams.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2yktyntqd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ckhpgvjd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2tzfdngjq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2elvyxcpc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ucossegm.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2vjjuhyef.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2hinvlwyn.html


<!-- 参考信息 -->