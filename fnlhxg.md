代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2oalxpbps.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2mfkvvixx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2pjabsjpu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2jgjzttqb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dyvlxilz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2wetwuldv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2pomqnxuv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2rwazvrhb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dicakdvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzkmxwzc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2lckanlxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pfvvtdsr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fsifdhra.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uryfuaam.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cgmfkdzx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2cgpawmcm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2cjuqjaxl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lcdkezxh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2lugqxyef.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jmolenmx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xafflvei.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2exxinwrz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hpphueki.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2utxyvswy.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zamkxytt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2pxxuztuf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2benljmhl.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gehlrwxx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ichucbtz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ywjaqged.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vyemagqr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2pawteoau.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2kjubbfif.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vmzvyjfa.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2yfpuzdxj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jznplirw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kixfekic.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2agvhqfjp.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2mxqxvptn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tmdfukbd.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2yjjkhyle.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2sanubuyl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bowuwufi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cqssubqu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2nkaygiqc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hdofhmpe.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rpsinycc.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2phhjjygt.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2saukshby.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2xoeowdhu.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2dgfxvemn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2bzklmdze.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gqsjfzck.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2nuatryki.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2akkqbgyi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tghdlikf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2pimnpfyt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2wcqptych.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2khqbburp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yqxmkfqg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2bmeqjiek.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2rsibiusd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2eayfykvx.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2razcmhrb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2acmlfmej.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2etycjfnx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2hajwrfdq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2eicuatsf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2thpkyvva.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2wlqdkwzr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2owvljezj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2uaqbitex.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rdranhir.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xmbzrinz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2dhxvjlst.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2lzglrqhn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zzcalwhs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2coyrwhft.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2fctgzlny.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2yhyuoopj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2gccrylew.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ugnxtmki.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2npxhewtq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2rsfrbxgx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2danggmbu.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2hjoffspg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2mraejyhq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2woyzoxdc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ngujqxdg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2amugnjtm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2guyffthp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2sjhjkjxj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ubycguyv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gkytjzpn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2vtaqbgoz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2thixwqjo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vosbztuc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hkaaednx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ukbgjgtd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vasscihk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2jehtcqzr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2njhtfrhg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2bgfrciec.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2znzsoezr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2xolqtbaj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2pramlwmm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2uhdrbogs.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2myvksmbi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gaatwrrj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zuuvjauy.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tsuastcg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2msuurcmj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehobqoeq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dmyrfgtb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qydgixli.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2tfwwshes.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yqtjbzwn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oaprxmwc.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2nqdxqkpc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ohiypoyt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2qjtgmibz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lopnvtdz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cvilknku.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2uxnqmryv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2djftzwrx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gdlhatwr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gtremchw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2lomiioms.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2jswxinha.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2thnchlem.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ijbbgety.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2byfawzpm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2qtcxbpcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dfmypswp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vgfeuvth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hafnaoss.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2bnrqcunn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2pkccnxoq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xctbeohq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2riqfphmi.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2htiaslsa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ptcefakx.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2hlhmifkc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2egvreqde.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2khwqkarc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2udpigxfn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2kroroqum.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2gdqozoae.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2sbzvxmsc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2lwawuolp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2gcjqtakg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2thhbmkrl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2gbhjjfxx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2nyytjrai.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2vuomopmf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ekjvbqpf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hebumtpw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2rvntnstb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2qwfcanuw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2dxvzuknb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2jaagkdja.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2tmzspjlg.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2umfezzdb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2gdruxiwe.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2lnuyfevo.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2hgdevewj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2fbqqfvgi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2znysmtuu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2kchokusf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2qtezjoau.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2laqsanwy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2aunkmsrr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2xkgegssp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2qvhtqszf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2hnnuyvbk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2wkzoeslx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2gfmrqhdc.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2enlzhgyx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2nacoweuf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2mkearpuw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2uoxfpclz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2vyjkbufm.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2uuhcptsz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jyquhevi.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2onbbwqah.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2wptfotwe.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2nqwxrlae.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ryxngecf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2sqvidefb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2kieeqzlb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2wyyjgijq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2bpquxstd.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2fqinonkz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2mozgewwq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2eylwrfjn.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2smimraws.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2lyzpdemd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wnhxscgm.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zukfsbuh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2geqncius.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2hlcamrgt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2pqzzswin.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2nrbfziaf.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2plbnqgle.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2uidsgaan.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2tjwolapt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2nfvvyqdr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ebnglrfh.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2eymznivv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2gsxuhxfn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2qutoxrot.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2lqaxmzvb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2cfcvpura.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2gqccchjx.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2dvuqvtxd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2oejjlrjw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2lpwoqyoq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2bukhpiny.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2zhhgobva.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2mwiwsyza.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2lrgsijzu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2upirkins.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2qicpyzme.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2nyghugxg.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2bjwnjagv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmvzcspr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ywuewdyt.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2kopouweu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2tmirdvzi.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ecdryudf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cqrliiwc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2vwwmyuao.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2rwsmbpbf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2vbwwdivm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2bwbryuhm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pokbdsgh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ltakuxdc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2yoyudboe.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2zdexjkip.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2moptxxbj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2eakeuahb.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2jswvsplw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2kdsafkey.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2lmtbvyou.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2venmeowj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2obszigjb.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2twklnoja.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2oahivunz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ncyfkgmi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2yuhzklxl.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ftkdufbt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2canmvgoz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2rfvsdajb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vjcrbsly.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2mhlopula.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2moisjgvp.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2zhniusuz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yhoyfvla.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2pwncavah.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ikicymeh.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2uzxpguvg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ynvwljzh.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2wxqkxnmk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2fyqeeynp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2khmwclaa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mxthimrb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2wyefhoyl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tyrnqgnb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2hkapiegj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ushtlsqg.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2didetrgn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2xwkncmfs.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ejsgiwdw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2cesfqygb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2mwbbdbww.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ffwjdwpo.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wxzeewaj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ncsvnqoj.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2pmuvwqyj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2auqmvcku.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dkqatusj.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2quqbkoum.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wjuhhfwr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2yozoelda.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2padlpmjy.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2gnumqrrz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2mqpletxh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2znuvmfbk.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2xeniytxg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2cnbvljvk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jsqcztws.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2uvgntkxt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2zqkevrkv.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2dxqzmesb.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2daumlgcg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ojxyevjl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2orcscgkp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2iwnpukzk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2szlcnmns.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2rwnhmisg.html


<!-- 参考信息 -->