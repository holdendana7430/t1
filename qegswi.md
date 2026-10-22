代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ajkxrzmq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeorxdcp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2knmrsmwl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2xsgqerpc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tqeikeoy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2trsmjshd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2vqpicbmz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2otftujln.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oxovmsyo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ulpcjexl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ahqpjcee.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ujiefvtr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2utcrzsnm.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2oplbzrcm.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2bmpkfysp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lullzzjt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tfcwmpdg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2eioavyzd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2okxhftwv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ydbrovwc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2yzbzktoe.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2zgulhysy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2djhayoyf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zyzxzusi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2jkvorjqc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2gvuyfacs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2fgtpqmvq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ifedibkh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jhlslkpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2encfgwjm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2djlltafa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmgkkaqv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ffshpvvf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2makbnjhp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2zqfnqxjl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2gmtvkfgv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2xxzwaixn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xevyolbn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2eunjoqjq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ulufkbnd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ngyrmojk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2bupqtrgg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xzmameqj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2deddmvjv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hxbbihxb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ftncgdor.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qflrahyt.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2aipoeulk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2okfnkdaf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ddfholtk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2uaccmukz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2alwtcwzu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2dkzgncur.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2mxvczqgb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2jepobzkq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qwpdguzv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2vcrplqmf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2xsqitiix.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2queqhxwj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mdpiwgyi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ppxbwwwk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2arnbzzah.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mugxsbhw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cibwdjhj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ittsygwz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2czaeuobi.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ludrquds.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2frosymsw.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2rrxanlfi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2uqmyvmwv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2nprszcuk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2bbchlcqr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2abssonbx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2axhsooap.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2zspzcjwt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ntqnvnei.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2zkkbknwf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fynnrxfb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2nozanykl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tkzhghmk.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ujimprdl.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2pglmihkn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2vzrtabva.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2keetczmf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fyrmpzls.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2xhnkpoxu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pikaszhn.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2eiwugzxy.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fdwrnbde.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2cowijpsa.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2afxgzitm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2xaoqkgbe.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zzvykssz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2trnfnsvy.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2zgzhzjfg.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2pgnqyzrn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ivdqwtpn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2epqhrojf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2gblbhnxt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2lgadkpxo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2epgoopet.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fmzptjik.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ztflzivw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2wilavxfs.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2euoaxjoi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dsfrlwio.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2oafvuhbs.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gxofkstp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2zhmgslid.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2zquodshk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2mozdovnc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2gmyekmfd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2myyavkou.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2jpczsutm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2albaqffw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2krdqawsi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fseyuedo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2mwmeqguo.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2wcvpyhar.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzzvqeve.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2spoxhamm.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbxqgrpx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2iremcske.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2pikidbdt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2bhynqypd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2oxquhziz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2cixaptwv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2kdayatvy.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vepjdefi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2aqoyeqgo.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2paydvdlo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2gwfayakh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2llvbsdwk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xbfvojjs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2orvzjqga.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2yoybebjr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2xwprsylc.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hriydoww.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2yxppodzw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tuauscwm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2euyrzlse.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zjmlvmyg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2akmszwmc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2nwahapxx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bmyqkmzm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2zsopuucc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jlmcftgy.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2qeqrzhus.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2uzumpouj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2yisnwgen.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pocgotnh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2swdqvnln.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2frbccmpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rriguvgk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2usfemuvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gsqkbvdo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2xuextzvk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2puyktspy.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2typykbqt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wduwrveq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qjxdfkgt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2pzcgfilq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2smcaylyi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ehptepxz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2wohvyaaw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gymwtjcd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2xkjzmvsx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2qdhlwksq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2johcjbjc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2vxzldpqh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2yzrkxoyv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2lgtdcdvw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2scmzkpwd.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2fmnsatax.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2yppupaxf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2lrbmaqnt.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2nyuzanpq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wlbubcfs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2buldwhzv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oepxabks.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2zwbmiclg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2zonmhhpf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2kzuyysiy.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2doirrltu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2apfxglto.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2vivnnjao.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2dbcqankf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2yurndsys.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2cqblfznf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2fzobiczd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2zebejvly.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vkaxybwb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2zjyewplh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngdnvfon.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2uetnxqxi.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2tlecskal.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2qeqzcozj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2omzsquva.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ufnzovqf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2nfuhgqfl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2hvxrqbxe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2skluusnr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2sflnqnbn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uafwcdxl.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2txumvkfo.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2dnhniskl.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2qlydcfyh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2vjtapwbd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2utletqqt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2iwqlvmil.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2difahzxq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2usqbxywx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2twjqwxua.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2nxdhfknr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hyplravp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2awbfnvxk.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2bptnmtvj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2bcvqrasp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2goksglsi.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2afauuonf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2zhuzwodl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2fxfrgtsk.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2wnjxnvmo.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2zgxjjpmb.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2zydmiwfq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2kccdcacq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2etrkkcss.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2zshyfzrf.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2pkvkeomm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2mzbfdwmc.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2nyhbtcnq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2rzkktenp.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ejblkhqv.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2zmnjuaow.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2mxttgfch.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2pdipxojk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2rerupxdg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ihkohhsj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ibnnwprc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2bpqtrpcu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2zaimkqhd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2hgixknps.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2nxarejkx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2otovinyb.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2sbbppmyr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mptevxeb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2wyaeoxrj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2hbwghqdk.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2cumcmyzz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2mhwsyqdi.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2xmmpbsps.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcjuikdb.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2gsjdxlrh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2mqlkpvwv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2tseoalmy.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2efxrlyxn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ceblrjfb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2hssetvyi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zcbjvtbf.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2lvmjlenq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2bwsoyhlu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2dygesjzv.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2dkewhted.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2aoamwsap.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ccetovua.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2aljvhclc.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2iyibdsuz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fijkehvc.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kbqbminz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2kogowueb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2pnnzopnf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2cjefisqm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2vncthwed.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dvzpnrmk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ehjbbzxj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2taqvwxdz.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2zkwpcizq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mrbcgyca.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2cpnbnkcr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2otqphmrt.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ehdjxqdw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2nfzizvvx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ncrxiyic.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2mdjsprjo.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2obvwmind.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ddhkczmi.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2bgtpqkca.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2oflgjjhq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2aihkwwpk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2xcpkkqfq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2lduigcjn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2kxajzgfm.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2lbtlnvph.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2gahjirht.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ftwjjaqm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ithwpdop.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vsjjnxvl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2myiheojz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2znwqjzdj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2pvqvayak.html


<!-- 参考信息 -->