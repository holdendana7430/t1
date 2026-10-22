代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zkxlzxsi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2fcbqlnaz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2bxificqq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2cunekvnj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fnscqexu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rmnlztpj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qhufozsi.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2clrmlonr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2tkemdghg.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2pazzjouc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2femksqzd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2joiujvdb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2neznxcev.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2bumknqrx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wbyqihwe.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2sbdxqomf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmjgizqw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2tfsquxia.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2tphyswvk.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ctgvarhp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2okqqdyic.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2tmexygtk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2awkyrvnz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mhsxyrzj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2juslectr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2acmkrftx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2stqlhlnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dosuantz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vlvieqew.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vyaafclw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2lraxqwxn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2bargmphk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2xpufhqpj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qodyoevo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2gtugeooh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2qaffqqjr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2cgknawwm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2buebhvzf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wyzbxydn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2muclgdkk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bpeauhmv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2blikzahh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vaiyqvag.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2stfzbpra.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2lgzuxuqi.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2epmntndx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bntatuzo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ucznrtzn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2gpxcmmxq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2uhirdgdy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2vyffqgdu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pxaekfmb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2golrnyix.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2byufltuc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ydsctnvw.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2snmcikwj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2uguuxpik.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wqxedtlz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lnacqfwn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2flrpwzxa.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2fzljaysa.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2udimqrqj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wtautapy.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2xpqpfkfp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2fmuucuon.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2cqoeltzr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2zswkygso.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2eqcjmxdp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2jfvusyng.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2paboeqem.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2eehjdtmh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2vnmizpdk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2idantmym.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nbwvlvrs.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dxamdezd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dazlhivp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2tylhfabx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2qnrtmxdj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2hnvtttfi.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lshecksz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2tedfcebc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2urzfywko.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2owbkkdsa.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2rtmjtrhe.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2jzodfcgl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2gxversad.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2sejzvvcb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tlgbyrtu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2awwgfuaa.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jnecwjfp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2vvfadiiu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mcdxgctg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2hykncqwr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2roibzgje.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2gcahybpq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2fdluddlx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2rbzqofnu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rynlacbf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2exuwhbnk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2zxaxqxby.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kofwioih.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dvppjsbl.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2uzmwzckr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2vrhpuhcj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xvpdbayi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2kwrottwb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2sdqdjovr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2facxrqog.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tfzlxvfk.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wrjtovbt.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xcndfvgq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ispuqnap.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qzthbkwj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2zaheqbmx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jovaslje.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltdmovyi.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qpzzpapp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyojcalb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2nnoburam.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqnfvyne.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2dttpjddd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2fnhnzmnt.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2vjuwbnib.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2goxfjbwo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ljwwrrcp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2juzflyav.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kupbyjba.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2gyeijugk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kiqcraaw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ghonaqad.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dlpmhdgs.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2yyohzzoo.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2qrdjjbro.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2twyrbjdb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zaqysltg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dgzrzqgr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2rebetmik.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gutemhdb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2tgxdogiq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ghexidrp.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tqcgvtag.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dlitaser.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2pjwjfqcz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2xbrcjovt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2kkwangne.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2dznoqdgf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vfchvjvi.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2zlqirhuu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ikawqyzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvkimhuf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2trjujnmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jzhlnejv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2liyxbudx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ptevvpux.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ynxcfvkx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jnywnsbh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zdzbnekp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2wqzzcemv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2kpipjvev.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2wsydnkmf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2idmhotpu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yjexczfg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2pwotqfnq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2raqsplqe.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2vxqvdfpa.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2wfvmmtsp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jxxzmizo.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2peoyxiux.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2yxkqrdwk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2qnvfeevz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ngihgnun.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2uhxxbivo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2eieswyab.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2axleudrd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2cxpeisei.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2xhyhyfbk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dxxovgfn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2hzjfcfpl.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2mkamjwmn.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jnrbsicy.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jjuzgspu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2yiynbtsp.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ukuwqbsl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2vmcylken.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2yeqxygrt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2txhmcvgf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ihcolvcz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mglnjksm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2eahfhigx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2sdsjtjzo.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2woreenoq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2dgxjtjaj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2oiltmezb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2qswvbeil.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ckuhdepy.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2koxeufrb.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ejxgnhnr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2wtjxigqv.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2kbtyjuaa.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rlfvcyfg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2rctqyavf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ynmfzkzt.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2rwhsjlmm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2aayiuqbo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2hkkbnaua.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2omlxaidv.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ccyclyah.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2xsujymjz.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2boiwapqg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2txomzofr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2qpgrlrlq.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hcyhjrbr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2fjxrufny.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2xlrsqqrw.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2lwalfnha.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ieroiumi.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2qwqehkmd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2wmewbqbn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2vzyqcpft.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2nhfehgxj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2sbsexrbt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2knohagrf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2gnofuafc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2tzvjzjwa.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2bznscnoj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2wvhddflb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2kajciuqq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2rjnvcxct.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2viliwxht.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2bqudmbas.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2gzbksrrl.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ergyiczk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2sxqdfrul.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ywfndegm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2pudvlrbj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2etqktaeq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2woenybni.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2oaqcsxvv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2plkgkfha.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2pttkyovx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2hhgwlosa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uryagfrj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2gevoddnb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2zexrynwm.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2gavtcbqo.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2tjsbyctc.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2miryftby.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjoosbwb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2dfylqyny.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2yzlhmisb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2tnjxkhcv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eszmicbd.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2stezrrfy.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2vxlvdgwf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mfosowuc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ugjiorfg.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2inpzldrl.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2libbecen.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2oovixlxm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2vwylokas.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ntoiqznw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2copmllrs.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jlmznmba.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eswfkzkk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eplrmzri.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2bszvaxsu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2hggfpypj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fcyupsfr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2aebtusdb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rezxsvxt.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ncvbdzne.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2xgiuwzrh.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2pbxoinbb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nnmejvqj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ekuktnsy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2githcqdq.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2vdizpsme.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2wsinajmd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fboxepjh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2vjahdvba.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2nypyacot.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gfdoubcv.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ahxxgchn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nxovhncu.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2qtfshjym.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2xxwlpumc.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2gwqofijb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2xlvqferv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2rtgvtsxc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2syagwyou.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2byjkkidu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2hwkipyqp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2qltlkpko.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ivohncng.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2isilxuqb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2airvnsgz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2nrqumfuu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2jaihbkpv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gceycfai.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2kopfmavn.html


<!-- 参考信息 -->