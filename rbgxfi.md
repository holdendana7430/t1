代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ruslsybj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sajdhasu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2pznbquve.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2frbfgtwo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2obazgztk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2hzszxtne.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2yxuhkite.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zqcpphiu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hkrvrovd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mxeltpnk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2bhaniceb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ysnbkgrf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2wrbtstrl.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2dxagajxh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2qkiscyqt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2nknjqhck.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2axpsqrtq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jqbxtnhy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2vlhfwuog.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cwhdtclr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hxaogxdq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tlmyxpxt.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ekebitkj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hhoktvop.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2enaferfw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2uwisyqlr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rdhrcvdt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2unrlaqzd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2xjvewenb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2wsaxsblb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nddyekyf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2qzfachqf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2tcmuknyo.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2pchsnxoh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2dfaksqdk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nifwzjon.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mehyjywu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2pgdzblwe.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2jtxcgber.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jvlsrfoe.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xxrvhbeq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xhbftite.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cctgcfve.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lttfxadd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2zcxxarjw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2bumjfszk.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2sckcyrok.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2zsjpoadf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pfmyrzgs.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2xzlwpudn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2giaboztw.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2urjrtxes.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tvadeima.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vjspvydd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2hszokhqr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2quctousk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eoipxahz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tlgmbovb.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qyqiujyh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2zxnmumsb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2yxvvetrn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2xbmhvcnx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ycypbfiz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2zolakerb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2rinepuwc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2bascxnik.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2opnpfxnr.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2mhnfrvzk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wijbjikk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2bpwxkufv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2mvvefmfu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2rqodineg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jixqulqa.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mgdjpcrm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2euzbhqdl.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2bhpiyajz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vfzkrwvv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2gewsfnst.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2eaeqhzvn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2azzierfe.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wuwrcqso.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2rtsyjgrv.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jqudqlan.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2unrctqdp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cihvwjep.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2nhwfdwyi.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ijcfqjvs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2pzjikovv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2purlqqzo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fijahitv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2apagwzvj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xazdksxt.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2dngkglby.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ddqhppnm.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2iervkbef.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2wptbemuj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtaopafy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zyenbrmx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jipvystz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fhzdnuvb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pztrvvfz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fcvmkjgk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2epxtlyge.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dxihksyw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mfeznehh.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vkbbryif.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2fkeowucp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2olfgmrjf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wqqtgeow.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pkizziij.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jusuyoqn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ayqlyjss.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2azskrxvg.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2aurbqrjf.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nafgyjzf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2wakztofr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ofylarcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgtfsrsr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bxgzazse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2osiktbjq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2pilwxbqc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2bbjemues.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2bjxhtjxn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zqlrbxyx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2drphlmzw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2emnkvuvs.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2dcbmpekt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2fpddzzrp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2wlrtejop.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2xmtbbjit.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2euxqwexn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2wttgywcj.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hthrioje.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jqjnxhtl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2boufrxxx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2gnxvxzfw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2hkzwabbc.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2dhjwuzsa.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2itqxbems.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2zksefubr.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2gjxacslx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2vifmrbug.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2tgxpuvjo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2wxmgjnyi.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2sxnakzux.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ughdbrrn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2bnxbpdkk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2tznrxhwf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2mkukpolh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2iwazrrpv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2kbyithtt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2wrlkkfcz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2xcpqrfes.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2dujridnh.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2saowcyst.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fuigyymi.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2cptyvwxu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2umqfttsv.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2bgfxcrzz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2wkhsfmis.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2gredrlmn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2nbzzuhcq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2cpfpqdzg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2sgmyzekv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2qxrobskj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2nmgkgvnj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2vrlugnpw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lhdgpdxd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ksgsolnb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2otavgftu.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2qjdhbgvg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2knfcnldz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2cthnmttd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2zffmtgjk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2bcodxfvp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2maxbtunn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2mlifoiic.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2wsqcmtqi.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wtvvdptx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jvzfauqp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2aodxckay.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2nmmrojep.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kfrlnvli.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2npstnixq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2gxpltbet.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2eloesexv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2rhkmxdmx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2tkecxwqj.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2zgortmee.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2zeungpye.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2wobxdkti.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2qpeqdtrd.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2wiplrhed.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2toqopevi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2xjtkhavp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ezpqggvj.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2abnowaow.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2anrlfpxc.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2jboaskcs.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2cufapmsp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2qrczgjyk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2fxemjknm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2apiufysk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xblgjkzu.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jmflyazf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2wxobufsl.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2gstitzur.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2uaohpvof.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2jfmwpqsf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2remhnnmn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2turqovim.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ptctegbx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2swpofarr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2pgjsmtjd.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2loshzonx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2amxvjodl.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2pflotidw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ysiusvcx.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2soelctth.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cjcoxhdl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2erkohhcg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ltrcvtst.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ymeesfmz.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2odlhkjca.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2xeixbjtl.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2nlmvavyw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2dsusfcdq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2copqxjxy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2izekbton.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xsjlfveb.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mzfisyyc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ngmbugsz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kjbwzvll.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2kjkrshsn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2gfrgdwsp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aljmkqaa.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2fubbqsjn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fuqkxkju.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2dwbajoap.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2avufoaqb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2xfnnonvl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mwsaayda.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ookckhez.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2mdnmxcjx.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2undudmsm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2dwepunyr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kkujlibi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2eqavihhs.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ytqrlgqs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jtwytutb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2cghkmewv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2bhncvkwi.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2fffqtjbr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2hfqpjxit.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2tfhlfobx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2huifzpdr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2lsffgjjf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2qzyfvwbj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2cfctrciv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2xzgxsrrg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fhojpgmf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2elaxxlkq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2nntenybz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2xmanvcru.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2porcvjbu.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ayqiowjc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hjyxmoho.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2mkkhkosp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ettinmec.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2bgzybabs.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ddtlogyt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2uhrzcsrg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2lfcqjqbm.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2cdlvkknu.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kowiqviv.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ryaolcjx.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2vitvrleg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2zajekpyk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2upophijx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2wyocnxsl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2nuozfqzx.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2xuoqulrb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2treqhety.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2cmuvgptp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2nfgomqdl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jqsgkyjl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2qhotijht.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2xedoxhqa.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2tbesgnoo.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2tgyzdtar.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2fruigglk.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2lshzwdxk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dwnfugpx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2wcqdpghr.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2weofpcnf.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ninewvjv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2dwvtqjlb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wdtkgyyi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2iprsktfk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qrkcncko.html


<!-- 参考信息 -->