代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjnbloig.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3maiijnmw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3yyeztoed.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3lfokwjih.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3vvrcpeja.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bfwivbes.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gncocrix.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3qgxmgxqi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgjkfifd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3hmjyxalo.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3kglznvbo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3knjhcnsh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3igjdiagw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3sukknfdy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3zfwbkmyn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pmnyifao.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3txzlpcob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrmylemt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ykyuxmdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jukaldaq.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kuhthsko.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fdkqbgxi.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jqfxtgbz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3vcsvoufu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3akostlep.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3pfuxuakw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3amjlrdrt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3glyyxtax.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3kwphnheh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3lmbmrgfp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nchbdqoi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iwouctur.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pexbduwe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wftprevn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3vrlokvfi.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mpiiinly.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ndrfcosa.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3swvxburt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yksmltcm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ftvkelqj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wycaqlgo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3dvtlqtas.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zatjqgas.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3equfxppd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3guyjgnzm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqmdvpyg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ftjftuzk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zbmswqch.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3tizycowz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yitxlews.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xqjggtfk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fblypcdv.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3owsqobkc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3bwydxlhb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ggwpknaa.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ccpvzznx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3msmwrndn.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3aabpuvig.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3fsknyryt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3oadygnin.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3yldtatgk.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ieiathlj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3zwiacrca.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zaphkknt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wbljcahr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3jfjdltud.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hjqltiri.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dwxxnpsy.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3tksugdad.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vkusocll.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3pyssyszh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3uvdsajol.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3blqjlzdh.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3jgrgasqg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3irfocnce.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3clxoyjha.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3idmjkcwg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ptdbozen.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3jxvbfhlu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gtnfatki.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nywkwpqi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bitvnloy.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3uonxgqlb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ofackwmt.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3cybqkydi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3yncuwlbk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qboqkioc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3pbjqyaum.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3tlejwlhc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wwrrhrjm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3lkfwvqia.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3rkrftgrm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cuelgqpl.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3dzdreixo.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3fsvmonad.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3xchdoxrl.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bsgdftri.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3uycdvjhc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3nydxjkzs.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3qwfvspwb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vrmzjonh.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ekmuhhtd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kqzsisqk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mxvfaexi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qnlyqeam.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3uplllsuj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ejrsvdwq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pitvezar.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hxwwnfae.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuzefziw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3vqzemcse.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsvdjvgl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3mwduakjm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3kymbzuvt.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3poltxgwt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ktcsecob.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3dlacecib.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3klkxcqri.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oisrvaby.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3siejhotk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3keuowcnr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aefzpcba.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cwfewuha.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tyxvofkr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3zszylhyr.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ckloetie.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3buasxqll.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dvijpoky.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ramnfoxl.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3olzwzvxe.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3qoeeehhz.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ckwljzlw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3pqhqexhh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pjthaktv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3juuderzr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3udjmbwtj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vvpodqph.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vkxwsucj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wunzvzmq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3onpeipch.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ilmneswh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sxkzwvfd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cnzksuui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htxuwiis.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3fadktulj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3hjfbriaf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3cenpuoet.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3cwcotvhh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qoytnoym.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3sxxgwayn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3xqhtspjf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3xpiesusa.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3rzzlhbbk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mnnkjzvs.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3lvmpjics.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3njiskzkt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ihahrnkj.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3inkxvpbb.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3akmbnsfy.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3rjkrchfj.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3gikcomba.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3yogtkjjs.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3guiqoeai.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3cijlxdfj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3kjmefmwk.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nyrwnsfz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3rjksuely.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gbwbqfpr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3dwwkghik.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3rtrojypj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3opzthksr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fflfsqtu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3sgsazlsc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3vebjfcqr.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3rpegzkmx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3yuxwakpf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ndhphwav.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3uuszanxb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3clfgjogt.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3domopuyk.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3uwmpjekl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3qeypbbgl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3vfqvxirz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ooadwfmf.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3bfntrmeh.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ayloqhzs.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3tegtydnc.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3qtlllqol.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3aqfgdwoa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qrnwqzzf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3sxiozfyk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xyljmdjq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3pzewypyr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3xyoksxkj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3wlztqqwt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3enpvaqpu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3lrwthwwv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3bxgfbild.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3cljdrdju.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3bjqsozyu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3qmjsazrb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3oerctybc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3yoyandib.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kollomxo.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3kcrhpchn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3bshzvhoh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ipysotif.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3qjewolfe.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3upafftyn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3hsrmuswt.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3buudnmtm.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3chqnokvq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3exhorbkn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3jjqmqhzm.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3qifrtdlv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3wyvtgbhk.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ikvahlfz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ihxsmdyt.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3jolhsfsu.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3btmimbmk.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ayvhwqav.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3suomojou.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3lbernxuf.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cgoumqtf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3wsvelntp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3kgxxwxdu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3rpryqsfr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3fuptpubq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ibezoxzi.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3kyrpvqmi.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ehjfdcdt.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ieehdrsh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3gewhkpfo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hwrkfvss.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3eqnuwvai.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3oeqcqcra.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3vdicgbyf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3qloihlwb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cxsybfpv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3jzxmieiq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3tebegwgk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3snsqwzrl.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3jwfjcdun.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3dycyefre.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ocxyzmwt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3gkfiztym.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3viulyauo.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cgpqrnfl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3pufgdkck.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3jdnfwikx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3tzparhdm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3xyheokyv.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xlmpfkoa.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3egcslzdc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3zgremqko.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bjhzcaol.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3obvjzmct.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3dbvhvbdp.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3kflelxlv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rlwdvkhg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3hxbkfrqg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qlxsfili.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3gdholgcd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3gyztlzsl.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3povkupye.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rvdulgkn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3lcwetffv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3mmojwroo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3fmrhmbet.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3kdzjafex.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jighctvu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ebbwpieg.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3lmqwejbn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3frxrsjgl.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3rywmtttk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3kgksttqq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3nzkxxcbt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3xhlhswrw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ibbwpekg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3dhodkhdr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3brvxiedx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3grpnhlhu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jrjdxvsk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3mpzifwmp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fagolpqd.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3jmsidvbd.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3vyhnoolo.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3lidcuydf.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3whsstjdw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3hlzpligg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nkaywrtf.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3pnxfqaqa.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3eyrqbjuc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3bkaisnoj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3iplpyymf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3cdhhwzlc.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3rynhcdhf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vfzpxxqy.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jhapcvbq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3rwowoehf.html


<!-- 参考信息 -->