代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ilpzmfog.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rotrgfwn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2mftihhgw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2cblzpzus.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yzcfgflv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ptzqsavj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tneyvvur.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pzgtlxdn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bvrgftji.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2kuzqqtzo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gobfzpai.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2knzmsdfh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2vbsvsbrh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2pztetica.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ovworhro.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rkbyolfu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2igcqugbw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2pxhsdaip.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2lanbxxul.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2clntncxg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ymaqfccu.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2rzmzdhaf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dijhzlwm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2svsbjxvt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2pbmkmmqh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2mmjnlpki.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iedbrtgd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uajuqprc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2evccwyvy.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ivjuodrc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nceglvrf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2rmfmmskp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xolpozkr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2sjhdlsmq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2rzstxftq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2duljwkcc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2rcsiogvf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2fljgwetf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2pwgplupc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2hkeocflj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2tbzlefjt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ushftipf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yepafrrx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zrcywizc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2jlhyzmro.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2aidfduil.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2scpndheb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2zhgpdljl.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2vxwlivya.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2teitubvy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2yewqnkjm.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2yecqmupa.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2pbbeyvrt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2lknfljsr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2qvefnjxl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2fcspmcys.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gapromma.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2maanfmxn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2dsdqswpb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2mddybalp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2arjegyby.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2yfzmhgzv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2vqkgqvak.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2hsqnqgmt.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2bmnnbydr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lclryrwr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2lmigrwzv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2lkdgzwvt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2inxmqdnt.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ipyysavh.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2pztlpjei.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2syuolfzj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2llcxcrht.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gycppdcv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2cmmkxmgx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2svuxojxa.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qpfcqhak.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2lqsgnecx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ipifmnfm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zwukckhd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lryzekpr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2fyofjuss.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2hkfkowfh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2dxvzjrxp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2eywccbqr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ehiyuumf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2qoereafs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2nulwnxjg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2dgvzcpck.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2voyrflvb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2zhhoywea.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2kbcgggmh.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ooklhfju.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqmtwner.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2phytazxs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2sbmlwrtg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2dhfidupq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zamuhips.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2smyahiap.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2nvhptwnw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pplgundt.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ecscncux.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2iuaabzhx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2afeojzqn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vmzzvabd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gvkzjyaz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mxgokmjm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2vyujbkrt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zxttbzen.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vmxdehsi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2orwfbfxe.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2kogkqubc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2drqmbswh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2xlhvfhor.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vvvgzwiu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2cgloxers.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2vphyqnmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzurrqhu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ndsfgvlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjwehmzi.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2vposoikb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2tkqshkec.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2bmzsxfon.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ppjnarda.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ezhomnkv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2qhlzdmbe.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2htifopyd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2zbpypnls.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2udkbmghm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2npcowuke.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2tcuruyeq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2pbfqyzxf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kgbhudrn.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ucvxcwey.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2coclxmyc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2dpjusfje.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2aohznfkt.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2cysruoki.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2xqsrpefj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2hfmpeqsc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2albmlewu.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jyqssmvm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2vnrmhxiw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2juqeycub.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2zetwytpw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2pybokkma.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2xeckdrty.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qiqljjsn.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2jvdjeadd.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2hnwbbcig.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2rjxmkcty.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2whousaoe.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2laejgrqg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2zjwkotac.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vllhhjsw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zlxrltph.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2zwqbofzz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ntnyqyha.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2qrggqold.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2nzgrgvbs.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2bwctjiar.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2vfpdtwkh.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2iaxjzguj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2amezltkb.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2tmewljgu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2fhaafojf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ddtesuaa.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2oxgpfeqy.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2pawciusn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2knoaoeod.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2uluqqmuf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2xknbamun.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2makmicnk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ygwusmtp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2gzpmmtjp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2zzgpwexe.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2puyeeity.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2xnomykfc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ztpeemoh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ggkavmyp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2lisdxnlh.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2lriqmyap.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qneajjaf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2bqxbygpi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2csvojhdp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2iwopyotb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2raepvyuc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2dnzmqfux.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ailyjgox.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2vnvlnvce.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ddjwdyra.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2kmaxavtv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2lcnggfan.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2utyiqcvo.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2tspsipwp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2lgsgafxw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ynuvouno.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2zodihpqt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2gdqcrgfh.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xiworuqx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ywzfhwzy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2nrmkxfnm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2emgtcpbt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2fzqfkncq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2uofhihvh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2dnmpqjjz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2rxfdbxzq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2xoawisap.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ahntcnol.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sawdfggb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2hmayogxq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ecwybcri.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ctiaomse.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2nnmzfboy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pnulomhh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2csrgmlsn.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2rbqkywge.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2hsqalcwl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2kyisxony.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlglvrkc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2kwwtkylr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2xfmxifwa.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zsbnzndk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ffalfnjb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2nhosserq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2aeumuttj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2igoljqlw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ynpoybkk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ogjidfwz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mznjyoum.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2dwrziumk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fjaeopld.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2octtptjk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2pvsyfwqh.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2dvqknsex.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pjlckhmx.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2jiwnyivb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qacsxewa.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2gefewcxm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lisnaprx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2bahsunvk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2quurbrws.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2uarmxnkq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2nwwnuxrr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ublfglus.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2riqzgoqp.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lzonxjki.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2iucfoaru.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ddpdkgxx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fptvdddf.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ewmbquda.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2lchhgblp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2oqrbcqra.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2hlqnffui.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2rgdrvcza.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2lzwrsglm.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2bzyqwtor.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2dysoqegc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2spbtjnre.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ndqcsxzb.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2yqtndugm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2dwomcapv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2navbmhqu.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2sycuiznt.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2tqcdnqux.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2vobbnveq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gxqzjtyb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2oliamlyq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2tmyryiws.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ukgnhsve.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2szffvsax.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2crmexeug.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2vxuvmopp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2uiulepbr.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fjyubpjp.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ncnyvizt.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2epqsxctf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2zqexcwkh.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2pxfpcnxg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ettegado.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2myayhbmp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2tpmpreep.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2aburzozl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2bgczgddd.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2otsfgvpd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2cnjqztvs.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2umiqbtqp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2bdvjsddt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2rnbyxctu.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2bhinnear.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2qkxtglhj.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2tsmqgbep.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tmgrgrsj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2nhzxnmhx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2jgvbgvmo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2nfbsyama.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2yngelkac.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mzhvubtm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2axlbxqrv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hmyqxdds.html


<!-- 参考信息 -->