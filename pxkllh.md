代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2syrexmwc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jyzkuvqc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2drxdfaid.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2zwrodeso.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qelsyfma.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yzxqygjf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2uwtdfden.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2kqhmijas.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2uwoayyna.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2irbcwhtv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wcxqseuw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xddzxijn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xozapmau.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2jwnbdnov.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2subzzbrm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ojdmuifg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2leyvdxrl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2lzlaoghr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hgavrsma.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2vpekhqwt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2bcwucltn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2nejcpjmw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2dgepaqej.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pehbeqls.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2qwfyskek.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zhravwao.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gcvehpys.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2faogzxea.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2gwojazgo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2qcmkeqtb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dyxgrwnf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fscvtepi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2fwrdmfrx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uflfcaee.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bhssoggj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2kqgcbuzz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2lapidagg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ykpgyryq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2vrrfrzwr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2oqzedlgk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2cvhnqvva.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2yrfquvyj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2idgehpfr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lwhnejec.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2assekvbt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2mqlspuwk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2pwmgxoey.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2eqvxxloo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ncsinkvw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2rvidnnqc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2tnzkimxa.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2acxidtjv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ababvfnx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2oulqvxzl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2spdzagid.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2kaqghsce.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qcfvclit.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ansleljr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2llrualrw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2pwvknlff.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dewfcmqx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wojylnmf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jbjhelhb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2mmmhbjuf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ttrcooen.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2swwncios.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2fbziyaeo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2phwsltwn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2oshuwoim.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rbssypxo.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pfazzdak.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2zxeonzvv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dxouyper.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dymvxiwc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2glwvmnlq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2moblcwvq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ueobhavf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2astzgvpl.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2xeguksri.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2wkxnvvtj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jznrrfls.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2tyhehhpx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ujckcgcq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2hxanhhvy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gdcoygxp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2baimwmhl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2pmoqkayp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2zdvnechy.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2yvkwlxsa.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxjhwwwd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2gilrsjso.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2mvvfadkj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2zikstzdc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2frpfxtij.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ullqiuql.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2uoktxaxy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2csaltasi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2meaghhin.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yssnsigl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2qjikhotw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wabhyavk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2splazhcv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cyumqgpr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2rxbuutfz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2sgbjbuzl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yvnwikpl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yozihmox.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hsjttdpp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xfqbtmee.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ibhrvxum.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2zhulqovh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2vyvmtafn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2kcgbeasc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ucchejrk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2efjvkvst.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2mdpeukrj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rkbwdwio.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2bembynrj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2eabrekls.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2kzppdjms.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2qqpobbqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wiiqwjyn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ynracbaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukdhxzyp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2qobnpine.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ucqgyqmw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2yybynyac.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2cqrdknfe.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2bzyafwyh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2buyhwwwo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2aemaslok.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2tridpuaa.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2czsklvdy.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2fplxawnp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2mmbcmjjm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2gyjatwqp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2rmgablzc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2koyljjte.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2bkaltdxa.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2uadnwpvz.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2lnvkdsap.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2lcklifsx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2snvpophf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2llbzdjzy.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qnipugri.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2eojrmzey.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2perjonuo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2stjsuvac.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2xlefqizs.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2zirwkutv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2egjztxtz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2eiakxrrk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2wvseiynl.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2tyobanfm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2tpxfxjbk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2gxbjsgty.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2iofmfddc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ylfmjjmi.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2kdneitwh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2kcveqdoq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2zsxreekv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2njeyemga.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2aimljtcg.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2pjolejom.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2rblejkiq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2zqzmuxqq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ilsstewa.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2fdfapsac.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2siuvnzpy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ftiqokns.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ygpeylfy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ofzafpkp.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2lbpvgyou.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2qmhhafkn.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2zqwpqdlm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2lxhhobmx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2dihxrrdp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2vlnxsedw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2uahoqibj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2fkoasgtg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2pwavmqxw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2iblkhfag.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2zfrnbmjo.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2yjbzpyiz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2xiylyeao.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2rkuwtgma.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2myxulfec.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2eplftquz.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2xvldnqjy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2mzyndlrq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2imefgjhd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2xxncyzle.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2kbqozaye.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2dtbsahfi.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2smlktybk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2aooyfonp.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2bgbdfvpr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ngslvyxx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2knnkmyjp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2idueomky.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2zdfwricl.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2iahmzumb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2vkypnsbu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2htcnvfbw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2wzwwoefm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2wiyucmcg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2xdkxgdbi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2rafarjfj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2fzbwpusi.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2tiocfovq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2hoknlzqf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2dmplrooh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ldsedlik.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2smbevqdp.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2hhzgyszx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2micklpfh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ndfxhkvn.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2tdrckuyq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qrwanljf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmmaddku.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2srusdayx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2fjqqysig.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ymrlrsqe.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2xdxmrhxc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2nvucmstt.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ptfotivk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ukndiido.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2yhbrtzun.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2dpdxewfa.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2qnczqbnq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ilzkwooi.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2bznkocci.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2scpdfpke.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wyksyukx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2cayblmrt.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zoakadkb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cmielfet.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2qfczewjj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2mtpwdkcm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2wulhlexd.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2egtafhnu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wdpmgpmx.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2yhnofiwr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2qksjxrib.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2aadclupt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2nvnnuapr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2vjdfnwis.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2hsijnqob.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2rorhcejl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2dhtgwgqu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2scvhxcma.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2qgahxlam.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2teriikwn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2seyspdll.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2zuyalqce.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kujjrpiq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2akklmrfw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ivtqvzbs.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2syceuoru.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2wtgebcko.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2wrodztbc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2rwdijkry.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2bilzzedc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2oxvqveym.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wtstuyui.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2zliznncs.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2knlnkbnt.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2atlnnzhe.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2blrfggyw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2iszkmhcr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2igngbbcd.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2gclovrqb.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2blmndqqm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2lbhbwhox.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2sjpqsflq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2droxdqic.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2omaeagci.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ieztphis.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2abtafahp.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2yfvxiugh.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2bmvpxnyw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2rmthkeav.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2xnbeijjy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2gjnwqkpu.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2suygmlvk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ghbcvycw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2oajnamom.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2dlhaptbi.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ufzugyui.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2kooscdhs.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2afjobnzk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2niwzeiyq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2lpdhvwmg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2jtdhkchm.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2fligwgbp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2abwrqpmo.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2dowvtnuq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2sabimpwy.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2yvufgekd.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2cxfptsgn.html


<!-- 参考信息 -->