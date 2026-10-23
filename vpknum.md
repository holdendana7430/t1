代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyouoniu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ysjpiivt.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3waokrprl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3fyyofwhp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vfzqbuxy.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3oealcytu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fhybwogg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3bjjlpakq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ktgvuwyv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3rzqnizek.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3kwxleepc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3aohlifxi.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sowgcpls.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3aufatsns.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3isyvopnl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3agdnebtr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3urfcyeip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3axzdmmmk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jwubdnja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3imegnkgu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qjcopwqe.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mqtkxgya.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nmnyrynz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3nzwhbdmk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ygsitzdx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3gvmligkk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3pwrsevla.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3kcdozdam.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3rvxjvzsl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3eyeidrun.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3elmizdaw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xmdpuazq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mmwepyau.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dkcnanfj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fviucolz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kbwcvaif.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3xjaalzyu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3lnvagqcb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fomzjrze.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3pkktgugg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ytzmliox.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3vofwulcd.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3auarehqo.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljwwlspl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3bwwsngsa.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3lzlookwt.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3asodnecu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3swmhkvyl.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3khktuewj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ncielqza.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nrypnile.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vbfyikrt.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3wnegenpu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3izoddawn.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mutrufut.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3hlfbaahi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wujdsxot.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3cdegdcdq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3fqkjezut.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3eiaqeoko.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3sdrpprvn.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3nyiuagao.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3uszylrzr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bdhloygw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3latohxot.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ypiejgfh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3yswqrotp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vvptbstx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3iwocozfs.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vmuarzbv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ezwijqwk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3slkkfcec.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3vndukrrz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3syactvwq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3cnbzptyj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ylezuowa.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nkikgnhl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ajadujbv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3thiidfrv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ssytwngu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jchiygcj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3egqqmjkq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wwzebzti.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3zghtqnoa.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3oyrzsnpu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3misysfps.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3jkhvzngy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ouyhgpap.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vhiikqhm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ncytivex.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3frapzbiq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ayawcmfp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ovwulhvs.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3cnwjhxgy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jczpykzs.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ttrtyofo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xgexpvyy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3rlduqfft.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3gcbkbzcj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3poidugcf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aflwfcnm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qpxdsupu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3zfwhgtmo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3aqdsjlea.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vpwgqcge.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3cpxdzoke.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3fxhycnkn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3rlllatdp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iiwscofw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajfbmatp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3owkehvfi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3fjbskguq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3nuodvrfi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3pygaaomk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pdzkrmbw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ksxrcrie.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ysijhoci.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqtmlkim.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sckfdlhy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3cyaeista.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3eosbdqvg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zhppofve.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lrczhzps.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ttqweznw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3wynvlxxy.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zcvbtike.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ipehfjct.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3crzpyelf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwyygtnl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hxljgjfx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdnowjyg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tmuvhuos.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lauhvngk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yaylebui.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tysqqgpz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3meqygpnd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nnagkzae.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3fpzpvifv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qsxhrgbn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3rwyxbxdu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3rdrltsua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fyqqcuah.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3smnckvmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qilagpni.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3loloiqce.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3duflzvip.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3zwunptli.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3lcwsmalh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dsbatovw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3oisqiuua.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3vgenurjk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3yleqtsax.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3wnhzvrxi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3uyjjvpei.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ophzpohu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3zzwahhkh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ixbxqhsw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3rmoyxtge.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ulkwgsyg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ixghypza.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3gvphdnlh.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ugjyuaag.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3yisaauwg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3obrfaekp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3oxctxtgz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dwancsdf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3zctrfaru.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3zgafnuac.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3yrfdkivb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3piwdbupi.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ghkkierf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rnitxmkb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ayfcgtkf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3poytynth.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3zzgluyeb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3yttjhhmu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3cxgouzzv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3wsqknxts.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3xhbykjgp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qvlznfkw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3whiurycz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3uhefxmvs.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3eovezwtw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3cofsvjcl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3rbazdanr.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ymhiehmn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3azxqgskg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3vmqscvbe.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3cldfstuz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3tucswuhf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3pnginpvb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xeepgpey.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3hknbdmts.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3cxczulgn.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3inhfybmh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3jgfgwtyx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ogrpaydv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3dtrrskxw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3xmjayluj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3xqzlugli.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ztirhkci.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ztiklwla.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fdfsedjh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ptnuwlpz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3jtapejmq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3xmvhtfve.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ncicpfxe.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3jslzuhkd.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3tqsoqsld.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3vlkcihqr.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3onnxdeww.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3srypffzr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3uokpjbpq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3pbntsyqh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3wvmpgtwk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3soarfdyw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3kizgpuvt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3zcpsqjth.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3feqfynhv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3vxmcknaj.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3dvwrkmwa.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3pxgtayuj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3bqkgbycq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3adywumpx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3llsynfqd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3sessuipe.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3rbydtimt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3mnxiucla.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ymitaysv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3hcigvyfo.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3jrtcpbmw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3qrbakupc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3lviyqfpv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3esdydlrt.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3xdnfovce.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3vgrhyzyo.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3bioiwldt.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ryjgsbyk.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uqtpdqcu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3mqgutips.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3vveidxtu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3qjoloyji.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3tvwhjwtz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3pvuhzzqi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3nvukxnix.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3nsftcaee.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ngqbgvpq.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3viojpult.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3amhrbeal.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zdenhrqn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3yikfprtn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ahtiumtt.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3btwvvizz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3eubkqyap.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3lbgrezqv.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uvlptrtu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xwvqwbnw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3svlhikke.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3falfubxe.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3obtikprf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3qmltdkpf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jwvglrmg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3obwulzvh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ogyotcku.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ooprdrqi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3btktcykd.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3bfkkbeqr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3tglocxcb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3vsildzap.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3dlferpzb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jaqndvdg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3qddkigzq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3vxwrrdwq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ezakhfpd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3shbnwksc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3bpuvraao.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3xmgvvtbe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3bkrzfwkv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3jzquefmt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ygmgdeum.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3rbdlhink.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3lbzgycmv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3yblxlswz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ztvkyxwb.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3cjmbpdio.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zqsmavzz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3hekrxrvt.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3gmflbvee.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lhndmhpn.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3vkpwxnhx.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hdwkfjzb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3gvdwlpsg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3gxeljzjx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3rpkdxggk.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3zpxpnzfa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ylrlfpdt.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3rtjmgqew.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3guuyuddf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vzrdolim.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3vpapiotj.html


<!-- 参考信息 -->