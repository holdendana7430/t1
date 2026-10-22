代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ssjgxyrw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ywssihas.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2oqvgxdre.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2cndafwtj.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2pqjxmnfl.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kijqfakd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2deqqabfj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2dnjqfsrq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2tbhcnobm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2vksnetgb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2crmunnky.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bocuuqve.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nyceubgn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2sshzetmt.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2bwlywbyd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nfgkfhdu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2piayoipd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2zqtjgixh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mirjwadh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ydiyeuhw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2hxqvviqn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lfcksdxo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2hgnlhnzz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zfxstlub.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2utmlsmov.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2bmoifxjt.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nmvxsmkq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bezxkrza.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2yonwhsli.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lbzccaoq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2brbvtqyx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2epzttasv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2iqvjdibi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ubkgpgxm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tzvumili.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2qgmfgejf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ommadrdi.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2prsrdixb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2klrvkoly.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2pgqpkcxg.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kzafhbtk.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2tdteeqlz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2mvdkuqki.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2unxodhsi.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qwpzrrql.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2adkdwqui.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ovkpbaft.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kdsgzwis.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2xdtxlqqs.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2bkarsuhk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2cmkkvhtk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2eqwtkyxh.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2atdrdifw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2orvfnkhc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2rrawbzch.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2jkvqkzyu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2dlovzppu.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nzmadrzy.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2nmedwnaa.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2gletduyo.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2maqkzuxw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nrsevoda.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2eotzmpak.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2gvglfxee.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2zfkchgow.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2hicgehpm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2beqpnlom.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2lzwihzag.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ksmbzmhp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2eyiuclln.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2xuhtvgll.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2bbsjapzl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2uvhduple.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2qcmgmxrg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2yfdrdyia.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2yowmuiqp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mkykldhg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2rjbdpicq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2irrfvmzx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2qjcugoqp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nqsxtits.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rmfswnaz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2aayeouwg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2grjnkiuc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kcqwdglt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2nvzypbyy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ffdluzey.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ogotiocp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2diarairi.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2qkjpxjrn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2czzvlqyh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2nvadncoa.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2cfnwmgfg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2oyaazkvv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qrabrdaf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2gwnuvpbn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lotrfhvq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jizgqoay.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hbnklhtr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2nicfabex.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ckfsfkps.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lmvzelia.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tvpuffqw.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ymhvvdyh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2csbhpfwy.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nsyxlhvk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2avhqyiym.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wdikwyyp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2fqdhpvax.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2iysxqspt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2oxfapfim.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2solcemmj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xscxdban.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kictqdia.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2htqkfeht.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2txfbllgm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2htjagdoa.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ahddezot.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fdqxspoz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2eqkhdwph.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2bjggxsoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwccmjvw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uvatiyql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dpxccuha.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2gucklgsg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2awnqyrct.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2gischcjj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2nxeaalyf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2umlsjpen.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2aunzupkk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2wrvoukpu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2bpdienav.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2uexmkugc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2otxujanh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2fqrqxyqc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ksfvqehr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2medtktmy.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2kpssnlwv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2uuemaorb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2qgwywlno.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2wgcvzsls.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2xdrmfize.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ekdfihpq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2tdszptzk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2fdczofqj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2lxqtbpxy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2kwfrogtv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ltmgocqn.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2repgtruq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ofuldypb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2cfkgmkab.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zsqwefub.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jovhbblk.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2pgkklpxl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2hazgtlto.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ehvqvcqi.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2pmjiynnn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2grazskoc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2gyihilth.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2kjlflvrh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2oizftpgb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ieszhjyo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2eoavylcl.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2qsxsfnxu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2jeypjfhs.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2tiacneyz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2vucypfnp.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2aruvbozu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2bqqojayp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2xnkdqarq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qcokdemk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ioywvdlm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2zieluyhe.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2zciathab.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ykbhykma.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2nwzmtdiq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2beqvhled.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2mwpxxtou.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2tvzpxosx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ytmsmuta.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2xpaqmkmg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2afxqdpmi.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2lzdjdigf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cjzvopwm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ymhghczj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ecwpjloc.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2skaxtujt.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ivxigddu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2cvlfdrxd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2tecefbsv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2xtcoctpe.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2vuagsjyh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2frfuarjm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2mqdniqxx.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xxmeornk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ppstgiak.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2eetjfxpc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2mzbeofrj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2nkdpdemc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2fjffkqop.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2pivelfzk.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2onlutfuf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2gavxrtfg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2opfoauzm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2gudntzgt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2tbarnxfg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2tujhykwr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2qejhxudl.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2sdwttmwx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2mqcxwmjb.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2mbteodxm.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2yrvgmgmy.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2alzogmfn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mstmucot.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2wccookpq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2zwnqljci.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ifglgrnr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2zmgfejnu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2vkiusfxq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2aopeyjfp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2attzfsnu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2uorobaiu.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2vjoxngdt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2eqltkous.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2dmtnkalw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2kwcxzkis.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jlbzutcc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mwudcrkw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ssnmdoxh.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2yxdngoxv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2mwyeutzj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2zsjqophf.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2roxlirtg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2lgjyidpx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2sshkcfft.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tyzjstcv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oeckqjze.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2cpfnfexa.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2wqvomrqa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ukprnxsf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2gfkdjryx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rwazhawb.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2iuklwhvb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ermnilwv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2sfirdtvr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ccmfkesz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2gbngpccs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2rifavszj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2axlognsd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2wcuxtugp.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2jakvneak.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2eqqsxttr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2otkpmwod.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fmejrrjd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2wozdhcis.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2lhpbxdcf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2kkcrnlst.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2fadekykt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ryxvzgzs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ulndhzab.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2vpdrzaes.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ufkbiwid.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2zzolgssl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2qnfqaraj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2dtfnvyik.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ygxvhsco.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2qjwptuus.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2mrygqdgk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zvgsxqyq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2mldfqbee.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cwaclxwe.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2icwwutkw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2lwaduufv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2rzxvxeax.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2atkbuuzz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2cwzfkdjb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2xuypcbfx.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2nrlgtlbj.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2upoimlji.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2zvrrwvii.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2embrccom.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2nksyyumv.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2hfbedfws.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ilaxhyox.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2uuejgtjf.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2fhhulxxc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2nubtntdk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2aizkkzcv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2stgotzgs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dwmmgptz.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2klomvgfm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2hlgsyyev.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2dsheszan.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2eigqajhf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2tnkgrjli.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2lxfuobgg.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2jyybaopk.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2gvzuzkwd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2sfgrfyqt.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2rwnujbkh.html


<!-- 参考信息 -->