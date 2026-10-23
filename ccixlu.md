代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qyosxgly.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3prartoms.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pnfxhwfh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3mlmoomqt.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3btsrwjsq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3siciwigc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ahiidlqw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3gcdijhuj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hpdvppia.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3cvqanrzn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pceoqhtp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iksbfbxw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3unitjghw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3mjuosqqs.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3tyhsgluw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kiwgueiz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3txohdeed.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3vkeccdlr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3gkghpjig.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3oentoeda.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3fgrlbjhz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3cujnbnfr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zvbpdbuc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmyglghg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3pownaxdb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3bxzuihuw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3bxghpjtb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jiyootfv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3xstslqxa.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pdhosyvp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hvnymvql.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mozzsbff.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3xgotcqlq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3kqqiabow.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uvbnjhwe.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3plfgaxns.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ciiwpack.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3xbiqslyy.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3tjkndfms.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3fawafkim.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rkfpvymm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3oqljgpov.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3uzyrdgxr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tebabjmk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qunmdngu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pxzoaogp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3qbgkcsgx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dbnlxkmc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3iqdcsxyi.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3cufrodzk.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3zcokcvrx.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ldopzamw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jnykmkgl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3tasiredj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vuujonfo.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3lpathevo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3apnyewhx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3bbaqsnny.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3gpamwmfy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dripvcet.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sfcwvild.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fhmasekn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3yuyigdzk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3yrfkhrfm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3kiemtcxs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fnqeorkp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fmdpdzvi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3vijwfsgb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3qvgnnfwa.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lnucsvio.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3litgnyyd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3qulesvzu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wfoycspw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ottkzeui.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ganzyudq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3yzvtraef.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3buuuvlmr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3flgiiazw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3vaueoiuj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3zklsqwhp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pnygjweb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zgvbittl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3qqhurfmi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3hyhokwwp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gpgsgibv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3qhmdudpl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fqymukdj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3xhypfcjk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3visbmrwj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3mjxlmchj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3qtwebkhn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3rrzxcsig.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3aykgdoow.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eykcxkow.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3sxibrngo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3vpxpfuuj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wtdhbtsq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yyckqffy.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zuitgkks.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3rxobbttn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixlnqarq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ufektgnf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bevduwzv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rhjihnyq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qbbzjdmz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vqipqzma.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3pdxqusgq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pdaaxhtl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3mafddagk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mskskwfv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3cjtapsqv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3keicydde.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3yqfaugoe.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3azawzwlf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3xkutaacv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3udwuhzgz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oaaxxvyz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3voencgex.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wocgirce.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3fenlqsme.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3pnltnvoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lzjlemrc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hdfaekcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lcgyveaa.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3pxjcyxnp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3fgnjobxr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3dhcqdtno.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lwhzdote.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ckbxdphi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ezdctqcq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3aqqzjlaa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3cdpqgfaq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3aetgsmsh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lqvvjiyv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3cmgopdwv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3opvioaok.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3cczuvtmt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3uormduhh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3zrmkeojv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3jigwuhbs.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3zeuvrlhj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3qqzalrxc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vreqzmzk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ttalkymp.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qqaayoll.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nvvdihrj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3wmhabrcj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ujvdgnmd.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qowunttp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fncfyhka.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3vxwetbac.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zmcnbecc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3rdwisojc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3syzshkes.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3dwfwrlhg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3rtmmxxrj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3vlabqrlo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kpjjnhgz.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3jlardjys.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3yizussll.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3mqbxglzd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3anmldgog.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3oaqhsszj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3nxcxbtdk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3irmdorir.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3dtabmekc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3zdumlvja.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3qxsecbhn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3fmzupfjy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ptviptmm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3agfmkejg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uuhckakz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3jcwaxdrv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3efdoquni.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3rwdszowj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3zuttwbmb.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xodgfzqm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3kgpyszao.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3lnqxkumd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3rmmnntgz.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3wzqjzxnd.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3tyikdxuf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3wehgfsnm.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yyozejpd.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ukyxiycp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3rlgvwxju.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dlalrbrw.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3eefceopa.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3xneajunf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3khsioptr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3kddtptfw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3gdcvwjfi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ssvtbosy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ddjwuphv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3xcneucst.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3dpyghpgk.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3larcnxlv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3lxlosnls.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3rnizbpfy.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3tihidjkd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3izgqihgg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3dstmbxis.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3tscshkff.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3claoqueo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ebeemalw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3sklicygj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3wwejzfzb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3pinozbzb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vurscrli.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3lcohzily.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3wcxknyhc.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ghhglqne.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3okcwcvez.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3owxuptfp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3mmksxazf.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3zxocxgrr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3grfqidho.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3vnvuudhu.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rrpftieu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdceikje.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3frqwzmhw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3spoozwhp.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3zlerqwoy.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3mlubqryq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3qopkuhyt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3sxlsnuoq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rkcpqwxj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3idptjarb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3oehcaman.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3hcdlxzmm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3bklydvmt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3dsxnzkfe.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fuifqpac.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vqomfvlv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lfvkcmjp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ugrqdbdj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rcakzeqd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xnzgjpid.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3nkiyzjeo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3plrcethy.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3lboiaiau.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ykbvjevv.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3skyxmilk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3nwlbruzy.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3godwughh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3fmigpjvl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3hxumvsif.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3fjbbfxqy.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3qnhlcnen.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3xfxlihsb.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vthnxnza.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3xwqspwfh.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3zvueylsq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xuwlwipp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3eztokmjt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cvrzzebh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3pzyewuix.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3pztogkik.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ihgomqyv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3wicmnukl.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3kyuvzryq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3aaaxuljd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3nspenvif.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3fpmlscgj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3fbljsvht.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3oevzebkh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3dynddqig.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3zgyvbttf.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3glrigmlp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3wtvsfpyd.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xxrgyrxz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3nvwlatxc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3jirclzoq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3bfdygeku.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3dvxiufbn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3qjlbpsvy.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3xoilbhcj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3oogccqki.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wyhkuqyf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ydqyohgg.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3fqyzxitu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3utnnazva.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3zumqilxx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3myngzgct.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3crpacvij.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3pckfcoqz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3rspsuwvk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3tzkbougu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3soytfkxi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kbcbyowd.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3xoxzbaao.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3okkfxgnl.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3rtsonofj.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3xnqlhnyu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3pveexadm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3bsboicyb.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3erbsmcvy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3vmpaouug.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3yojpgqho.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3eiwastkl.html


<!-- 参考信息 -->