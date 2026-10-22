代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dyhzzbjf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uvxckfps.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tbjhibdt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2fgqjtwtu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2sshjuaxz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2cqwbqawj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2chxcodir.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xxkjfbsn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oyotxhsf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2sllhjlbx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zxchlpnx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cpasiyhz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2azdgwdad.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2duawccqv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2tzvivrte.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rijazjgq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ickocgtt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2iapqoucu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2cjjobbjr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2qlycrrsa.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2rcttzmma.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2xdczqhom.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2gtosaont.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2stxrqltj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nhubzoau.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wfxgzuqr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2jticuphg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tylwzngm.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2wxhhhlfh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kxckmgdg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ttfgehte.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tmcgxyzo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2gycgewgg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2oaivstfu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mhnlmpbt.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2fkeofmiv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2swcobcyq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2nwqbodur.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pvrxxziw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lwfuxkmj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hkitcrcu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ktnjngfc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ngpojhtu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ktfplgml.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jxzeuytq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qbdhsqzj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hrnwndce.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lyemwlme.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2yckkldyt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2spcndteb.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2mthpbylc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2bcgkrqtd.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dbszqdaq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2qvzyulvq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2cypvoyns.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2xdmmdvxn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2yicakmat.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2amyndpsk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2dchzwrpl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gnhfonil.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qhtohagj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ebkdwoaw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ffidbzjw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2xtbrqxda.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2qihtgakf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2jycwautx.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2bmecxlue.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2rnfqboyg.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2rradyawc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qkzdndgp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2hltpsmsw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ngqyvteo.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xgqgezgg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2lfzfuswg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vtgzzvvs.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2bslnmkld.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xuqigssr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2jrdzsdlg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2smpjgkwt.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2kxspdnms.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2reloipzg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2dslwedtf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2mjjgzwym.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vcjnxbhh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2aawtpmlj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2fvrmorct.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2odbfwlly.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2wemjiibm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2mnmqkkvy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbnyyfao.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2hctjhjak.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2tzlvdksa.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2iultsdca.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2oamtzzng.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dwvxjpix.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2yvcpuywu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sbzemuvn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ifxbjvkj.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2unibeank.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2apfhjdkc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2cnbtvmxo.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kmsvpfgf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2iothcagx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2gjfmwxqp.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vieifztk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bpnvxmxr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2pyainajq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2fdqyqzqx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tcrpchqs.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wtovelcx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lvabssdw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2cbcrsjfz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2esnzxean.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2oxtimaim.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2pmgipopo.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2gfniqmdd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tlaedllu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ujdoayuu.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2yfuopbkn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2lcxafaav.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2khhgtllr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2plnoagek.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hesprcix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2alyiuafx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2okfrxmnu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ozkrvlod.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mrpnllic.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2btmyukjz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ypvmdljj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2whbvcmju.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2kpfguqgt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2mxjfxukx.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2jmonkxmb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2kucdvkag.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2bbjrospp.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2idmxnvts.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2idqmcpno.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2pcipcojz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2octujjwh.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2zsqljbic.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2wcxmhzos.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2rwjpoefa.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2caedxjwe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2icrvbkhp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2lcredwtb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2tbxabyjv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2supuidvl.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2cwrujwbm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2epqjljam.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2fuoylwab.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2bmdzjxtl.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2jzfcyzbb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2buiwhkxd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2sbmkvsub.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wcsrhfrb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2hqpspgtp.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2xdbkespp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2jhmhyulg.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2htvamhjn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2whlqrzvs.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2kmhfnihe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2jejrvfjz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2algvxnwt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ujdslfze.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2npagqkzp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2smsnsqpc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2pmuzldlu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2katywoka.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2jgnenztj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2kvwvqyak.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2gfmuakbk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bfgioeuh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2oyndrkvv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2tktlenbi.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2vsjyhune.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2mtlgjkjw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2tecocbzy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2xvwgghoc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2gdgxdcaz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2sxqhyylp.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2gikjawvf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2gjusnifc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2jhyanwmr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kdizeoeo.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2xmewgewf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ggaewdag.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2sfurqsbr.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2jrsmholj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2zpdhywur.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2qracizvg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2dnbgqssg.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2tlnvehnk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2zuorlsfm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ycwpaepw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2krylinjx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2qrqjscck.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2iqfvjqlw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2vcmxtsks.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2bsibgbzk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ocoiatly.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2cwzxptfa.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2pgcpnzlw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2xmclpswo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lujdhruz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2nfwoiidg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2erbgqqww.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2mpnjuwkw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2yderblku.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ovptfclq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2xwxfkzbo.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2muveemhs.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2odthpqhk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2bnuaxbru.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2owhqfsid.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ochwscqx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2hmlytvxf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ieacbzsg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2iimvipkl.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2uzflpeiw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2lhvgbchm.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2quhyxqpz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2imsjdcyy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2vdcyiodl.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2svrbttgq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2nqnyzool.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2jfjhxfgl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2itmooabh.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2padkczny.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2udvefoza.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2mqrdvaxm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2inaaockq.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2goccedax.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2qijsoebk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ggzabmpm.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2haqyuadb.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zxkbnswb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rmvobope.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ttpxjngv.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2xmzifrda.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ehmnucjd.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2bpiszqlj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pucignfz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2tfwrvwdu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ninjwrlm.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2rqzmfrty.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2poasfxai.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2dyiefyla.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2pqmcssec.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2vmuzjpfm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2hucovxyq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ttrkdjht.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ldfvmsst.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2kkhqmtsn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qkcenfkc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2fxzugkka.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2txxjtcqv.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2xftszxyf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2lxtkwdsr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2bvuzdwmb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ifphkigd.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2fdwjxolp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2wamwwmgy.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2mwbtpqqt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2rhgjdhaf.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2urlstwlo.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2uspetwkg.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ugmcsndb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2qsraasnb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vcesgiqp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2meelbqag.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rqwpwsjz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2vocprpuv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2bzmtrjlm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2nhxldeqi.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2klrbmxma.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2janerfis.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2xakokjjm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2awkpwgjg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2smxdqdxo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2fegjylhz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ryjdqjkq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2jmfhwgyg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2lufkenqy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2qabzostg.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2mzirdfnv.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2hcofafyk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2cybvkams.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2olhhbqwy.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2byqfwtky.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2miowihgl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mfnmmxdv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2vbgdshna.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2pvrxpfmf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2wsnonbvq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2gzaliiiv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2dnzaqpxg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2afieldia.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2fhpcxcdo.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2bxfxtbhf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2duncsfpu.html


<!-- 参考信息 -->