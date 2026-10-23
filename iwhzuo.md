代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3guchpvxs.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jpgfzjuu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fmkbinbl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3xkopilpm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bjjucnai.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3gfxqgbcm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3gjmzgjnl.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3zmechysp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3erjivpmj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3tdpsppeq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ujmrlgka.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ouamnwso.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xkusjafr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ilkrxqic.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pppearsm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3gvcmpgnb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3dfboykwe.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3kanjmtqw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3kpimfkhe.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tpfdelok.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wlkfvfqc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3liwxcwvc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3lbxcnfdc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ixdtrpay.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ubymlbdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmhtwxpu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ffphbkld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aullsvfr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vfinndkc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nhsosdbn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3achqvapm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3tbbmshzr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3bptpvjbq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mykoyrlo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fosjsnnn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3cphhhgdr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xncbjzuw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3qxnhmqjf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3maesopsx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zklzojtg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3whvkjdmc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bmvfnoab.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zukdwuvq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3iufphbvu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3yyairqir.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qufpfrfi.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kvojovmy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3umzksdwt.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3nlcgjejn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3siizudhf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3hvosadyc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qqjeqitx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3anakfujg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pulujbyr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zlmqtxhy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zqqqtkei.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3remvwzea.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jjhhfywo.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ydlnysso.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3slcuneef.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ugiqyifb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mxzuisax.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ngigusos.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3gjignacc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3nhgcibda.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3gdywxzln.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3xrdhbygz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3olnqrbut.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3xvxnhzle.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ddqevnms.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3oowfsgzi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3qpvazjra.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tubvpawb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3jejrvxqi.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3xagrkzyl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wievfdut.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3einatdds.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ulxjxfqi.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3nfljkyya.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3yoqbiqqj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3vmdvztph.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3zigellgw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bbtnfbpl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3trvanhpy.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qxfmkqgr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ajqkreue.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3khxwikeg.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3eplozvnd.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jziabsei.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hjensdov.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3yrpnsuze.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3thsoyfsc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3rkijvtjz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3kadvsjob.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3zgdviaxh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3glnzozhh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3lryxtxqb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3hhabuuac.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3xcrbiljy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3fxmiagkg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3taeesyqg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3xbclpkgi.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3dxyiwdhv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3bcayllnv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qctnetsy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ewqnjcze.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3sxjyhsqs.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3iioyfcfu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bvkvjlxs.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3tjfpsrgi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3gkfgeboe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fsbxskbu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qmwuotje.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3qfdecwmr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3cncvmfgw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3hgtluqjb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bhhutqpk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3fgqxwwco.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3gwyectan.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3duxnmzke.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3jubmxajn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3sdxprkkf.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3zziqaorj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3fwthamgc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3qtthalzj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mssrsfpp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wjqbropr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3fhbbkoxf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuwhjnax.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uidokexm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vnsvhumu.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3auuhzkvf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3craccsda.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cvtaqlwc.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nbvhkgcm.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3sgleeixg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jcpjficd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vadogvml.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3khjzupxi.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3kjfslngx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ofoodkjw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lilutqib.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gdpuqxju.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3kdoeovak.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3vykkpxxs.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zciuwbgi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rzqumkxu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3pscwfuky.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ppmgvbuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjktcdfy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jpxaexhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxlgzqjl.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3wyqgegyq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3vadcbzmn.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3kjzslwtr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3nannzsqt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3puuyybsl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3chcnwwmy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3hjmtgkyf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3bhnjhbkh.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ouegdtju.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3opydxakq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3hwruftpv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3lbllzple.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3dckqzvvw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3szhxaniu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3wackxwhk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3mpyqhfjl.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jwchhlbf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ydobyvwa.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3grjjosqd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3lgueubdo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hrxybzfi.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3surmxlez.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3lnexgsxj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3lwiqfhky.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3vhiegumz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ogeurwsj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3zvgbxsnv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3nlpqjhpf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3gcuiddqh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3zslojuka.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3hbrxgnwm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3pyjaqrfv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3mrdursji.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3owjpwfuq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3moyqcyrz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3euygyhqw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3dduycogb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3cgfbvkva.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3yaabvyvd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3bxztkvbu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3cqxvrdgz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3airexqnc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ltivihvl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3nrfueaqn.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3gbbgtyqs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3kasakzva.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3hawdcrmr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jiubxrjd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3hsipwxjz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3jifybpsx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3paylvexe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3gqmewzbd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3giurtpdd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3dssvrmbh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3bocxrkzf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3cmmjofwa.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3bsnisdfe.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3kernvpzv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3nvjadhyq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3rtguotft.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3xorlnkax.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3xqbqpwes.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3rdzrxtfh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3uqqsdvby.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3coarluko.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ighlxcbv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3aenpvvdj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ioagktit.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3pkxmilkd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3fhohlnqj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pkwmymvu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3obdirgao.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3gfkgizva.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3tlcznpcm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3jhvdqqnd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3jxlotzwa.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3dhdbhoxo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3lxxepoey.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3cbtzdxjq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3tpsysoai.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3vmczjjsx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3jwsfwipw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3kzvbfyhy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3fmwbkblk.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3iyvcfsyy.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3xwyivahr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3yogqhusa.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3lokvlrti.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3nvglimxd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3goyrnwwt.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3bzrzbgce.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3eyajdikn.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3lzqafyro.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3uruageql.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ernnywat.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxgqybnb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3htcngggk.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3grcotbgj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3eogqthks.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3huumqfww.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3xjwoxahz.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3tuondnog.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3cytuydgv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cpgnbyoo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3welrgkeh.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3pjbwbncb.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3vgnrlzes.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3dyipffve.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hsyjalxd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3lcuqkdel.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3zzttlxqn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zanlltbr.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sztxbkof.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3qfmbtmgm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3wuzhxstm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3whnitcaa.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3vzimvpxt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yhyxzwtc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3xlplijqe.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3vztvejzg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3sbfeqfkg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3sxukuogk.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3rxmubmcg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3luenbwaf.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3pwniulbk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3hjrymlbx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3oizwrjrn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3odvuoyuw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3caafzsdk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nepscuzw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3efqmimuq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3eblrxcah.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3udfnbodh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3fdknjyvs.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3hftrikrr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3wllhetep.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3raatcxmh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ekmjviey.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3fsxseptv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3bjgmcjdf.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lnmtabao.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vpazrzjv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3exmwwgoj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3vxzpaznd.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lkekhkwr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3gkojcliq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3byaycrtq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ofibniow.html


<!-- 参考信息 -->