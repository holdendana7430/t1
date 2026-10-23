代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3eauesadi.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jwlwmrbm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mwodvjtx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3raoissqy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gkshbimi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hzcayxyp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ctyokvoh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3sqvkcgjt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsipnspi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3xgckxdtp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3kwncheka.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3bvppftvy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pmeiqinq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3fnzsgfck.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tdwpnydl.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3bnbipbsp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxpnajro.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hltzweee.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3szyahalw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3rijuarar.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pmwrsisj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3umyapkhl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3rnvkoiuu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ijijgafr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3eyxgkuqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uekjxqbw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3yntcmhet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzrcnfov.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yalwqbkt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3izzmxsyy.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3kowcggpg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3pckedvwm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3qgnysxzi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3grrddzfr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3klzczwbi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ffezvzcr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3npwktdlq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3qfbketla.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ikicgefg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xsskqeva.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ypzjrsha.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3lsokkgdj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3shhfveni.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mbhmuscs.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3uxgjtkht.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ukdnguzs.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gdutcnbo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3kvfydejx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3awulgdhv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3gdbytwpq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3skusmoey.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qkudodej.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3shulkycl.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptheyhge.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3dyjfiiiu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3uwqxbxep.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3jctclkrf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3czkcnsfl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eiasigqz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ghxasbcu.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3khovhjmi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3qgxhsjos.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xrppcipy.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3gagtyoud.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3uajxwwxp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3jakapslb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3oycpvahu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3yecusfkx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hcbmsozq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zdmvesgw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3hoaapwij.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pgbzslso.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nzqdzdfl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fwtpowhh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3tpsoukvm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wytmvkic.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ocpjbzzx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3osjhiofh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3kxrgrfya.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3hqqvejjf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3rzbkywxh.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ynwmapkw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vocmjjoc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ooxsgptt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3janorizi.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3uqhxdail.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3uislczbg.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mpngjqfu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vouomsad.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vejzmhgf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3gxdirdir.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3puuihewu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ucndyltf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3gxgyqutk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3orlpgqye.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3foynsxfo.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vurtyzez.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cbxifrqz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3efvufqyn.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3gmnihhnl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3eaaeilxi.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3gxqgidtv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xcoynnoe.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3obxywwur.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hlseoequ.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3dugeuatc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3rhtysvtc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3gvzcraen.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3loohmqhq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3dhyhivhm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3idahyatg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wjqlkfbk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3foaamdvc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3imdrivdj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xekjjjgo.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3dvfbkaeh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ylowlrgf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3toxiqoqs.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3bzjwhbwu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3wiojdmct.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3bwtxomvx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3dkhfwvod.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3kqwbwtsc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3dncnmlgh.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3okhidieo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ctmdsxad.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ruwwcaoa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3fjwpumkb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3vyyhiwcm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fmshvlsv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jeryapkc.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3gerclcdk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dfikxiql.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3oizirxpy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zugzhtym.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fvqtpfcz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dzvcumsn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3udgrdnvn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3lubggzjy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3iugfmfon.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ynqcbgbv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3clujigtv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zhstjybh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3roskzitj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3rvdbhrej.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ckgnbwpr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3dcuuacii.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3dykrjjod.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3hrnfjfcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wauziwkz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pkqxjstf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omkadzsr.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ogvhgcys.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3yhxzbhtq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3zgkxabso.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3peigolzm.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3hiawbazk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3mhypwlgj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3rztldloq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rebbkvcw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3mfpimisc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hxlrawdh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3wznzrshx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ijfmosek.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ktowdiqo.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3kozhofsq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3iskwenvg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3xdktbzcu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3mvpfupnc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3dzkplijp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3dmzediha.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3fkhnigzw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3lndkbore.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3uofcxoce.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3lawqdvcb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3wqsotxnj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hjqqlgss.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ebejycnt.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3harafvlu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hcfyxely.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3drzvgkxl.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3nmeallgb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3jkwmsesd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3vbjghrtz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3vljopnir.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3nymxhubw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3zeikczkz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3cdzyarxi.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3vbxgsmhf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3xogudyoo.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3nllhdgzo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3howvuhha.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3vfkntlwk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3aebklqor.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3cbvtlrun.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3teopkiqq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3wdmjxifl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ofoytdju.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3amzdlofc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wumriotb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3gnykpgcr.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3kjlryalk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3mmynkqku.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3dkeqrvuf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3arsxkpvg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3zqfslnkl.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3xnxpdvcz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3zwseedhu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3desscpvg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3lvjlduau.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3gtppamwv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3enutjowe.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3gzbzdqjn.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3mvqvjboj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3polpicrf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3llhmnvwl.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3myfbhdxb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3osdoffwc.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3njzsdieh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3eyvuymuq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3fydqrfcl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3vyutgqnl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3yeazgrfj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3zbwhqdyf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3qtvoevpf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3iwjlmyno.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3jzfeiapb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3kdpytzpz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3fhqqzivr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3mxmyamii.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3zaddiwwb.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vkowyneb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3sjckvunw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3yatjyfkk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3acxclrhi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3cqfrwcov.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ontfrfdh.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3oieewbyw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3loisusez.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ofmrtjic.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3japitwuc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxudnjmo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3axiubarh.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3dvykmiqe.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3hyxmwhlk.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3rjkvscnu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3gxnfricc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3msaokvbj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3zcdzrtdi.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3qxzwfhwj.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3tevonzxg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbtsljtn.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3fjemwvyc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3wtzxqlgo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3znmbxquv.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ukstkywm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3xhddtmxq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3aayvbpov.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3lumwvfzj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3hfbmuskd.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3cwajzgpf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dwldnwwk.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wtdzyhel.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xjcqondn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3unrzzxal.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3hvnsyjye.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ynkunvko.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3qvwelakr.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3unomcgfj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3agiqqpmv.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ahzxdntw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3qkugkhph.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3urjukpmz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3pcgptbml.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3bzmiubkc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3tyyaopcp.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ntaorwey.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3vfqeglzl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3unceozwh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3bnfizvkj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3gyrycyqi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xfakhssk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3wuuyugkk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tofdjrgz.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3bgoddltw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3xenrujjk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3tmxmxtct.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3lyizyyab.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3padbmimn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3mdqjnvoh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3gorqyixk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3zulmcmff.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mqvxgqzh.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3cqwfrcxc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3mjdxqqjv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3topdgbqz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ybdrtdpa.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3bwjigmdo.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lhbkbddz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3pwwcneuw.html


<!-- 参考信息 -->