代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3zvhggmty.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3eqkwgoen.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tirysxud.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3nszxejjk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsykocms.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3kbjjievd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3vbkkyizq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3coaigbvw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3bejjnpgj.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3khidhegy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3dtafdbmy.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3yutzalfn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ichfmrpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhpfkpcj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ndntykrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpxdspnw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yhhvfgdl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xiwmajga.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3gwuqqgdu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3qiezvoyh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3zycjwsgm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xmhxfgil.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3nxiqrbfr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hethtilj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3wdxxfpxw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ntwbjpfx.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qtnudoan.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vrtrezkn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cvdntesu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bxopkncj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3umxvsfcs.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3uvsijmjv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3sxinktpc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3hhskkcgp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ntpfhlqf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ephavmtc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vgbpezid.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3vuyodjag.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3dzhwoztu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yyrgslpn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jujefgda.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3rimkelrv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3iwyxomnx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hwtgdpeq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3poulmoby.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3blbmbfvn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tgjjahpt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dehpcrae.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ayrjbpqz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lmmnnfpc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3igwgonvt.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3nqhnstxp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ciwuanwl.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dihigiqp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3vngmszuo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3xqzjbols.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3fjdtkesf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3anbazdmo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3bajenlcd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qwtylaaj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ippgdugk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gvzpywoz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jskpjeku.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vgfjtfqi.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3minhmvlq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3mxamztwr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3fzhvqxje.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3otbtachl.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3eatldgqw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3hhgekbqf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rkngkhpf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3bsquglox.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fyoembbe.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3njeaqvrg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3rszqwfen.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3vunrqogi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sdecmtst.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kwpypgit.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qxbdnmgv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gqszacyo.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cjsaaimo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3uyvbmvtd.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3wcyfimwi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3vpydchsr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3irbgcrxu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3uxnabpln.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hqajkktm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ckcrslxq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3sqpmwlxi.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3nwywmjfl.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ghzfmkyb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3zxurgspb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wxbjjqht.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xkqfpshe.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3yainykxb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3vhpjnqbf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bkjengej.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3etgmqwlr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wjrzukdf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3gezemune.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bveddlgd.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3texaxyar.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3mgxphupp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3sretqygo.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rzfliwus.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3tssjrhbm.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3hgrvrglc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpizcoku.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3fwswpklm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wifajcra.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3lelebaci.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3emqlugrw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3suhoqznj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3iprgfwfv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jntpmqrj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3fryygsus.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3visgttzp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hgxztqgm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3onlizljy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3uorlwleb.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3esgqsnaf.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wbajavnz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zraeqxdt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3woylkcgl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jlimuabg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dqmmjwli.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3bseaxyom.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3lzfzxayh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3aqfqrhxm.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ndmudlzi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3egsfpkdf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3qpbfwsir.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xitvqjbt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3iuwvzfcg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ecyymcoc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3nndlieff.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3fmhssxle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owtjztbd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hlgsrsaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmaaqdwt.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3uvxbnkoi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3irmwloik.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ftbkdvpr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3dadmhfgk.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lodvbban.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3rbcusavh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3rmqlywln.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3cfqvgwyq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3hwdfwumi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3befhnjhb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3szsyrzrq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3etoisamh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3furujhxp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3xsxfwuuq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3etxejwdw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3gqevtapf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3fdsiqloe.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3oziyactb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3jplmewyg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3itrbkniz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jcptyavf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yijiimby.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3zibuifsz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xptuamwc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3fzxjytvm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3qyxfmtgc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3gbdfiwpr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zwesjxqa.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3jfhbjnaz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3egtjtdwr.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ouojxaur.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hxftwpyv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3aznigdle.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3tlhayzgh.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3drahvijy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mshfmddx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ohjeavfo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ihzzxjez.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3edlmumby.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3htmklysh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3uknwkgnm.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ahdypaez.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3svtgbcfq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3aupmqeyh.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3seelbeig.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3mqayhsmb.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3fjtbbsus.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yuemsgud.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3qwddptav.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3yhssssim.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3evrdfosl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ggzgdzbk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3bxnmgrly.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ijbzethh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3alerlwpv.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3jdcayajx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3kkkxdscj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3hgsgssfd.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3gcaswwjw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yogelgre.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3pbpcflmk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3xatyyxmr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3gjyidhfw.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3itafqymk.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3faglrytq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3eggvwzrk.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3hdgoixjq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3fwnjsare.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3bxruhkpk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3pkngcqbo.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3hpuczcnz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3qngkbnjd.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3hvfkagoc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3zpsvspxg.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3mrvomnib.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3hhcboaqs.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3bbqnzxhs.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3lmnrnqnq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3mtsablgc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3poaddjgv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3zpvnkxwz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3hmpawwwx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3aysfvaen.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3uvewfcca.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3iialvies.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3nzevjauy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3kjnpmkpc.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3rdvkxrjk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3omomffqn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbisysyj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3qzufwwhw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3xqrtptmf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3eymgzvuj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3vvhsiijx.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ijbvcwdw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3qjeionnz.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3zlmfqwqy.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3zhvzmiss.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3sqvrhugt.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqivbpvb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3aggxrtag.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ajiumxqm.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hvyhkmcm.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mtbddtlg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3cfxjvaji.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3aciriqyc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3byowmbep.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3vlbekoev.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3gysobfjl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3pfcsuxih.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3gqutlprx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yoyhrfyu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rakyvzlz.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ngsvzfgd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3cagqzkyc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fouuebgb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3uekorrvk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zvcaeeki.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3azdvimiu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hbzqovvn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3lxwciban.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3fiafygpl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3vkzppgua.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3giksejxh.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3rrgjjivr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ujgroiof.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3xbgdmazw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3usodgian.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3oyvusgye.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3eguvuiae.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3aznkxoyl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qdxmwvwj.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3vhmwyoir.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3zojnvyit.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3oqwqcawb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3hhzxphxj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3tckllulx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3bzvdonvd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3hcgamimk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ourlthwv.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zkgzocbc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3rmrxionn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3eylbxdgu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3unyjdemv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3vwqvnknm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3mrgecbau.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ukodurll.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3vhzijvmj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3sqxocnaz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3zskrgvey.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3tbgjodom.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3kyapvkjp.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3nhdxvatr.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3hcsjjklv.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zzevweop.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3frsgzlpn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3tponaynb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3pvjuryja.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3imhklslh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3xehvapor.html


<!-- 参考信息 -->