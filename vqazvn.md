代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3zbazqtgo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hcrmmzqf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xisszqvk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3shgjtkut.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3puubimcg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vslssqpg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3yntwhdiz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ivqouyba.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxeiopwe.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3phshrwll.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ayehrqeb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rkqrwvxp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tgchxicm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xaxvfzvx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zauozymc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3akoownmo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3nolyfhjb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qqdzfoea.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xriiobez.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3qnusvmmr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3npewmmlv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3akvnwaov.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3aongauqy.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jnciauyp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hbpryqhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yowhhtie.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3nslplcdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yssezuum.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cdnsnstm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qliwlofb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ojogkjti.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3qlutftqd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3rybmkjrw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ohistqsm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rqmpwtza.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3tpzfswuf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3dompeybs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3cltvbmau.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3miqenayt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xgqqlesx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mnihsgjf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3bdfqmymw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3dhqmxpet.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xislnnii.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3knwrhdvk.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3yvyklmah.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xdjhzqbv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3oamccryp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3cxxylxxf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3lbuhupaa.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3dqbqauzh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eghntvvf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hmdjpdsj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3edzzgejf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3xyyzskia.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ymuwaler.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3wzrufaqv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3sintnpbx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uwxjdodk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lnakdhub.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ebvavpfu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lrigzdbn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hwhgiklz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3awkuhyet.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vfsaykyw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3inaltlpp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3fatydxxu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3twuqnsbo.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3neblcrfh.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3emhddknp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3gdndadac.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qnnbkpju.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3lxsstkpp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3buygipix.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3nqjleion.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3svrukmhv.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3jmkjhemy.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3nksjsebp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ijeezbtk.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3axofsont.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3vjjnaxwl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3zymspvub.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ehqolyau.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3noxoxeaa.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ffqmrejk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gvswsukd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3xnlrjrpq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hiyuatmp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mtzfkbvo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hrgsnnee.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3sxccdvce.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3lczpjpzo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3evyicaxw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3xauszoaq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3duskwaio.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3hyjyxwio.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3mdnhtlag.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fxyinvlk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ynracrjb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3gtkardci.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kgijttra.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ooszwcbr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3zifxgxzf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ykiwvkzt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ksqvqmuf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3bmhvbazx.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3tjsnkhuq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3slurdxwc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qgbofqna.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3bfgkhfpi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3fgszqyav.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3sgplzgmx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ejignwhe.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3lquuneko.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ajghwrgb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3gvlpckda.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lajgoxzo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftvmwoob.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3linvbbji.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wudjarql.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3hdbzpmsa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fonazpgw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3grkzpkva.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3chiqfccm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3vfztalce.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xxqttgmy.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ykwbblgz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wmmxpzqb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nltswsbb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wjfhtgva.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3iyosndii.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ijdgdkyv.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3xpqwwdgs.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uakiqycd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3eygxbnlt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3yjrokspy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3dinihurl.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qxxluaam.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3fvokplmo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vjcddiwc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3uqcppgby.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iejlwimm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hrkjvnqw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3pkqljlxj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ihojfnot.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hpuinmau.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jzaqvmrs.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jwzinhso.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3xekljrba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sodnnygn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3kegfrsfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3auwmxatq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3zyekakxf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3koflgtvk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3vtgvtytl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3fpvcoiur.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vmmwftps.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3siyippwm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3rlateqml.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3oxlvqcxd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3dedpdajw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ifdgsfyc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3pvbdwwos.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3vxxxsyff.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3lrfwfcbd.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3wmlfsquo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3axdwopcl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3xzoxwfpg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3flkzpfzp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3nrbtiuzo.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3tmfatzmy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ocfgouva.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3yprbjvya.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3uojgcrsz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3fadqypow.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3xwzirvws.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qazmqmpn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3bzapkfni.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3lsrbxlju.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dpfojsgm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3njwohihu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3mocxbkhj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3rhdxkqug.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hhhflxtb.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3rnessplx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3qgbfwjfk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3xkzefeig.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3dtpazsnc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3bhwsboch.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3bkgjssyz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3fgiaqxnm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3jbarxpbt.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3bpsqokxx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3vrnqlnuk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3hbnkhtip.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3bboahokj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3bgyisirn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3glcdwfrl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3htmfopdr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uxlyfwsj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ccdorgcm.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3exvmurkq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3jxeehnfd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3zyqvxwso.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3aiyuzogc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3mjswxedj.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3yxbqcval.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3vstqrchu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3niieawkw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3zuhumwvt.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3uipqquno.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lcielleo.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3gcopgken.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3wmpehjlp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bsasgqfu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3swljmmcj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3oocvzyht.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3lzsglpro.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3aycebzil.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3vmgkviwg.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3fhngburm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3vbuqozvu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3xwcsbuod.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3himqhqlr.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3qaxpagkn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3nkstezed.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3jqjjmytg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3dudllzlk.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ooeqjraf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3dcrujovl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ypnezwux.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hiyzeovi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3nwohpmrp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ofcwgjyf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3cpkljdym.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ldvdeoer.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lgvudcra.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3lqratock.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3bovhbgme.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3vwvasgie.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3hgbhneds.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncjsnchc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3lvnacayh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ecfkresv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3gzggpfli.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ezcottvy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lkdjyojn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3zzvjhzod.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3pnxhzoqn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3twoatzci.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3aesfyxfy.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3dfjtxmbp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3khvzvjqf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3tosprjcz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3uexnyljp.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3eowodkgp.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3oaapzxlu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3hqxbmiqi.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3paxiaivt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3jwjbldtm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3yxjgxavu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dbbzxkhi.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3zmfiwcvd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wrezxubd.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qpgtjkol.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3iuccyupl.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3khygyazn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3nyhxoptq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3hixngcbu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3prrdsvno.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3wnxbhakz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3mbicdusw.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3clzrawiy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3btiobjff.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3emcsccvd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3nrmurpgk.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3xworxaic.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3hdeyzwxy.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nmzjfyor.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3pshtzsmu.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3brdocnxr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vdwrtjli.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3hdegrivy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hvvsqzjx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3xiusotcx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3fokqunne.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3rwrvzvlr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3vvzplwxu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ilfdgqob.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3uwgxskxy.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3hzsozyoe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3osddrfdg.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3kiqynvvo.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ynotnblb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3pkhtbseb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3rbwefezm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3zelcolxs.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3xhcrgfmc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3iagjzfdg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3tfvpeujm.html


<!-- 参考信息 -->