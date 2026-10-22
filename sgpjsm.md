代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vouvnwxr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2krfrwexr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bdhtrwvh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zocwltwz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rzmyljun.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2wktigpdy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2diocquzp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mgrdhopg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2wxtchbzr.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ergpfqbs.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2zzvfjrqt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2tqhwmfca.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2slevgykx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2epanwdsp.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2pktucedy.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xhvkacja.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2afdgzzni.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2kkrgzaff.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2mxhmhxls.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ipupsyvh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ontwmoua.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ouncqgbc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kbkxgbrf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wczndmdj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2uxluhfix.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2boepyvqi.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xszeiezx.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2jrglrbpx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2sgogxlim.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2vmxfbdcf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2cyccwtdh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2iozkobcb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pmamhtzx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2eotxzofz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2zwbbxmcc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qdlqphkj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ktkissbz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dujytrml.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hwfqtddr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cpvzuxox.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2xawuzvne.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2lcaedayi.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2remrrayn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2kjuvrmqo.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vchxijgq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2eqrrjybw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2nfnhjbik.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2gscxqbvj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qmaomvrf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2oqnfsnno.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2krxxecft.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2hrdrwyzg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bbqthisa.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tgxqmzjs.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2zwicianu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2lmeaysbc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2zhxxsiqu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2wgsbcbpf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2bbhbvkrj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2kgkoylal.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2dhooapar.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xqenjsjd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2sejcrjjx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2slkdpuip.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2tlwgxnzf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2phslrqol.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2oalmcudt.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2kbtzgjxd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2yvyqkcvd.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2efmarqxt.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2bjiewvdt.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2zevpjtwu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ndgcxmgu.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2teknmbwu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2dpplaguz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2cyojduej.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mqxhlazw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ulnedrza.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ubcwslwn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrknvzrs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fsyvtnxp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2zrikijph.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2gxynnrjr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2xxlivppd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2dmwiodzn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2azdlpouq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2iafkmbml.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2hsfdtrhw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2gcewckme.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzcohasz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ilgtjlfb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2rufmrnpd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2fhkwgotj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2khsqjxbp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gaficxjo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2oqmxnphf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2slztqiyf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eajcalnu.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2cozjvuck.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wugrnsub.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ajrevxjw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ttvyvfea.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nggwoopo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2fhcxazsh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wxvvgdrn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rpucaoqc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2yvjrorwv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ztvtbhqc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2xclxzxqo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2mjwshbkb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bvxpmkiu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2udfrfvpr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2bahdjllm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsiwqpbf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vcfljyaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2njqsgbdv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2buplgftf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2nbyecyzt.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2uylysymk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ndhxqtcu.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2eflvykua.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2bsdxmjsy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2gnktgtah.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2tdfkpjaz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2xvylgodx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zgrzjdne.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2cjyfffrk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2wdgqkfwr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2qbvawslk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2tgccqypb.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2gpcdunsi.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ufibuzhb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2xkdvykrd.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2vxtrsqwz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2syfpvwxd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2zrkdrluy.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ugblqylf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2gwkhwavn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ahxfmdnb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ureyurmm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2rdzganqh.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2fqdqgpgy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2mmmzgkia.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2eakwqlib.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2smjnpoat.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2lpqejqwm.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2srryrrlj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wswcqfge.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ofeylrpz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2pclzlojs.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2sfgbfsdw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zixsdove.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2traeknkm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2jajzntzi.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2jpgbsyaj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2mkhjpmbv.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2gccjfcxo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2qivrphvd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2hdiaxdkt.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2wupybrxv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ubdlnueb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2xjqmnowg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2wyidfzsf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lyksnpcp.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2jxhhqizb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2seqhphej.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2symzvodu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2rzxrycwd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2aiqjtsfl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2lhzxmhgy.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2uvbjoqfh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2glaoxdad.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2xcjacewt.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2scvmoero.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2tqmsthho.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2stjltkqf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2hqthjukc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2rwfepyra.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2warrxlrm.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2waqozjzr.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2smedxqhn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2fjvrqmex.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2mrmngrhj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2pcrrrypq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2reyygkrk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2fuszziho.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hpbbhlmd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2zrdxxjve.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2bnjukvfe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2sixoivii.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2vrkpkrdi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2vudgscxd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2vyoxzjlx.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2zulklqtj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2wsauujrk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mdasliyt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ikyeqoqp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2vhhocjdl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2vonpshst.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2jsvgorqy.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ancgenur.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2defyvmme.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2msxqmhep.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2yrompwci.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ahnrlqvm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2osopofxl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2xjjulrzf.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2islektpn.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2yalvbhow.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2qcgvpvow.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yjabfepa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnhyzudi.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2owjmtkuc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2lmkbzcof.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2cvoyzhcw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2vdhtbimd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2fkcueoyr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2uxcguvgw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2vixqtqvi.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2uqhkxxji.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ebhnrbin.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2cogmddji.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ytzwqazb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2mwmcndeu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2uodhalll.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hgopotap.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2nztrhdxc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jddryslb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qazmkijt.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2gsezgenv.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2lljpeglr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2turszhdq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2athtsbul.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ladxdqmt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2gifxfabw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2btbnktvp.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2vdjmjsdn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kkfltqhq.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2sadccffm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2psqtctmc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2kidulrcg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2mgobslsg.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ictbexjn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ygrengem.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2poxlyrjm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nelxkaaw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2zuvrybum.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2phjiihaj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2snowythb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2jywpgnoe.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2hggsvvbb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2mlifoojl.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2pdkmcmmg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2emdxvhlc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2njxjyboq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2mdjvrbwn.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2uvewdzjd.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ullauppr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2gwmnynzs.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2cubknoto.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2cwvlsmle.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2qtkyldwa.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2sjhobrpe.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2usxuzxcm.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2gzbbkxoy.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2qgezhras.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2lnevwval.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2suqhdfxb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2vuaijufg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2aysgsbxa.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2mkwurwsy.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2eekitthy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ifqkcaji.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2yarzptkc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2tddlxktr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2gvcytabp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ytxyytrb.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2zdsyvlkl.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2qknaewco.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2gpgpnqkr.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2kjgqvxhe.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qotvnjwu.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2llbpwbmt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2bbrkocth.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2trwpzjfm.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2bahvnyjt.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2jhfkkrav.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2twgjeptz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2byucldnn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2pgbbjquq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2yczhoyyr.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2xlwuuxnq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2nwyxdnej.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2foiymkab.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2fypyibfy.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2egjbihpo.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ifxcsika.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2jgzszlcd.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2vnisbzfk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xtlyrbki.html


<!-- 参考信息 -->