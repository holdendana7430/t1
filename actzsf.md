代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2zgnjkoco.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ttzmfnty.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nzzrkrej.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2cisznfpl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ipswcubv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2fwhwlyuo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ufiiyhft.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2cidwnkxe.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vxxfgvah.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2fmnpremd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vekbisff.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vzorpfpc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2skqtnldp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cnftihac.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ythgsuxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmlfxpej.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ufauynbb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2awfdacaf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2qqsmtmqi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2diacxall.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ieuhwumu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gpoittup.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2txrgidwe.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2tqiardww.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mebwawlx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wekmqpbv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2mrypeswz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rmajzjzt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xbeozhon.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xreiaxas.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jucyoqcc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2euakrmfm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2gbbuebzp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2toxrcxzx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lnzofbnq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2qgvvracj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2jogqonhz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ydlvzwxo.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2yntkfadc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2scpdrhxn.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2mordccvy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ughzxtpa.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2qevuenwd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rnmgzozg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2jycbnylc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2husbxfek.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bajfhfoi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dttolwrb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2vfzfwdap.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2phypbhky.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pbmlhlxy.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2iwtdhbyc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2blhctrdb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2lydlgbac.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2lajkkcnx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xfjmpnwk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2tdcijxur.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2wxjgbfzy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2nldcwydp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kauzsbna.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gzdrzasy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2gqjdlybh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bbowqowe.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2biasukus.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2tlhafzve.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ierepfiz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2bihoiikq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2cpdoxpps.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2izgktrcv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2apyajddx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2nqzbyawe.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ewmnxafe.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xcaoryjc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2nstvezte.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2dnunfnnf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yrpndymg.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nhqpnmfw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2npuiezsl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2tobuacbq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gappfywv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2iejhgkhq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2wnruassl.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2yboaymnl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2dqgnnpjw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2utfnoatg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2flgysdwt.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rgztajsg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2wolekaqf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2emstvsci.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2kziqpqxj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2grzyvnmq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2eykqpkno.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nodyqxzb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vmqplxgj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2wivkdxkd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2hprpteao.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jterwdeg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2aqixuvzc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2pgjrieel.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ppuxxquk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bmbuappm.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2nwooiqfh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rgayjdbt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2aftqkymj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2avjuxycd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2xfnhgqka.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2jvnvgcqv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwjzvmyo.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2efleolir.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2jsbleclw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2rryxchvx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xfcvkijr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2tnqmguod.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2teevrirr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pqgpvxdc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2llvhwdrr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ozpltsmk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gvabfokr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2aznzndno.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2bjmfcpox.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gfaynooh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2urpqkhem.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sogbjhvn.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qruwckeg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lqmfeflq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hdwxwqgq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lgmxdexb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2sgnfhcxn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xirttopc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tffoprqh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2sedcqxfw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2bzeezaau.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mwgwckgi.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vkdkahgk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gjoraqwx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2iywpsthn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2jxitbfpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iflqheaw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nqceepfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ijculvvz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2gbrymzvy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2qaiqpbvg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2jnosyfmq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2zuiyqezv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2gkicynnb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2jfekvoch.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2jwslmwbj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2tkngcybf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2drosaphp.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kwveuksn.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2pfrzibmc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vfjronxn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2tpirtmtp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2sbpdijve.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2iljlddda.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2cbczydgs.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2grmmlpgr.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2vidxebub.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ntditqqu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2admttpjh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2mugdsrjm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2dhikfble.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2wccsorbt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nebuwwhr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2yjbamhya.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2kxqpxymp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2umhrudww.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ujidwqym.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2agobrlll.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2tbepkban.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2svpqytrh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2krjslzna.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2huglronz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2gbsxkmmr.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2rwcvknib.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zzlzmzly.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2zrhypzqc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2kiiwrvtv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2vdvlqcfl.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2vifpjylc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2dremnexe.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2wexotrmo.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2uzdljkvd.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2jhrarmfc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2rlslcjig.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2kviobelo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2njfnrdac.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cwmnjncp.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2fnxacpdi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2bjldiijo.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2gfhegeyn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2kixwtxgp.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2rkwirnqs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2gqyzrzjf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2kivoonvf.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2dimaozba.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2mwrdwblh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ebrmdivt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2fueiqrhp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dxdwhxqi.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ijyjgyvm.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2juzyjfdw.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ukmecuco.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2eaamizff.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2eavoztey.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2zgakcova.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2rgqvawju.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2rkupopig.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2nvndftgq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2qnkhnewr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nziozucf.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ijbkcjhv.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2cscnmmcl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2naisvptq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ntwskqwr.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2mubkbypm.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2dqrwquzs.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2gwvuxwmm.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2obipkvql.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2kebcnute.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2qxueylhu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2lzylsetz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2geaznoai.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2iusekyuk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2vjirczfv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2viofzyxg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2vrwuaqgt.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2mdxemtov.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2yfnezvqc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dgupkzbs.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2hypfkjgk.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2dbpqiqdy.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2obufjvmb.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2yozsbrur.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kwnzviov.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqgywutc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xqumydof.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2rsvgzsla.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2hfoyocik.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2pmfqmezr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2bjigutxy.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ubgzbyvl.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ovopgxqr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kdmnakpp.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2twivrrmd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2sonfxhla.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2nqbfencb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2extvatss.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dhhzuplq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2nwfyjkbb.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qcfkhaez.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2opffpmdo.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bvenfzxq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ciaazbns.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2mxqaihdt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cuvrwupl.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2vtchvzsv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pfxtjpld.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2vqzyjycr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2jzzdbsst.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2tgqmkcgn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hmqgjxwy.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2estuktvb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2sypchcpv.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2jadnesrz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2esgwgudd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2yfeabile.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2htmnhzla.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2sqhzqxbn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lbrqcecf.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ssgycsvs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2xuzfngnu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2yuomfgyl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2kajrapvp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2sslrgojm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2cuspwiqc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2tyourbwi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2inltjhsj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2kejkksmj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2npfcqoqo.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zzjtemvj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tqncuyek.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2hmvbxmfk.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2eqjybaob.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fspxcibt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2xzaglkfd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jnsrngbl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2jspsfglo.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2icyrjhsm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2cldirmqs.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2rjqfbqrq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2rhojixrm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2xagfhvzk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2wsmwqxxo.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xfnqfkhs.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2aqaaikuw.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2sdjtchel.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2nhdzyifd.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2zkjzhnre.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2paixgoeu.html


<!-- 参考信息 -->