代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ezxweaqe.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cdtybvxs.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3xorwalrt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3tucunqhc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ghdhamau.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3tbulikwm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ctsuxayz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3xxowskfy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3vevhapmw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yykopnpi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3grfztfjc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3cfdmktcv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqfwxqkj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3xxkiwjak.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fdywqwqv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3isngrxpt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tcydxtrn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3pjwvzrbr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3zcwhazou.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dreralew.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jfvtjeyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnlhmcdb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3bzjxzkfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zkiibsua.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3njaxzjuh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3samqxvmk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3thxopxuw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3gyksilhv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3tqewdyys.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mdnsaywn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3tysoxvgz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3cfnrxshe.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ifkzlkir.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3hatlwxlq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3eozbygsz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nbltohft.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3shfepdex.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3eyosdimc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3bxtkbrrb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nerioyzo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3lhgxhkzm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3yygalssw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3gaqvpphe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3fiakywfh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3uxffptbv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3aykrzzli.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ztpapbup.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zwzssajq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rgrgmhby.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3niqnzvez.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yizmgghc.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hnwmfyag.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3kzqttxwl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mbijtnwy.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lfmcther.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iracoffi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3cpfcsxne.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3byetviqe.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ubmdxnzp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3lopodlic.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3aosqcnts.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3dlymdeub.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3nddbherk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3itrvzpri.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3fhwxechg.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3skmfmumi.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3dxywjmyc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3twdjqcda.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3unaepstx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3brlqpihv.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3fhqkbwyc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3znqvtren.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3xsflyrma.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3gsmqxycz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3opxasfup.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3auwzxrpl.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3sukprxdq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3rhxfqqyp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3hhebaihy.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xcikoncv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rvyydazk.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3gafgswev.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3tghsowai.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3nbbnqfnq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3khsmkqlc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nubopdzf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3amsiozqm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kxtupvmg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vpsowjbm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3dkiazjww.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3blxckjpf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3iixfazkc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3rvrmdgtg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3dywtrplb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3wlntinmw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zxmotvka.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gqdyhuei.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3rfzwmjev.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vpflisbd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3imtdrsee.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pbjsrgys.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3yzoegopy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3kpfiljfy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3kjhqehzl.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zrevekgo.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3sldctvhk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3szprkynx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ngubyxpq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pshvvplb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ldqommlt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ewdwmrqk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcytnnnz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bttvbuee.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgtsibie.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3jsyqnoxr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtrjqzaw.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3wnddocum.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqbmvxwq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3iqqnnmgt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3klhhuvna.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zexfbxje.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sgscdehh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xbsqxvlh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3slznudvq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3urokqvxu.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wqohlzqj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qaumqfmq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3urgviwqv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nudatuyu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tcwxkqad.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3weygjfly.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kymenqro.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nqwtdppy.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dknmthot.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3xqmdcfzc.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3deoxzbfq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3trylvnod.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gargwdur.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ckzxmmpz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3roonrlsz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3hmfkjeeu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3zdvwpwai.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wreldgro.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3vhywgbcw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3gcuwazwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tkhgxjqy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dneqcsme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvshukgz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3hzmjepty.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3msmvguzb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3imisuycm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jpgqbget.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lugnczle.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3azxpnhxo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3dbghfqcd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rwsihbqf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3mxklawci.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3bblchhky.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3gsxvyask.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3jteqzmqb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ilffrvcw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3mvfppeyh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3vpmraqzv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3jgsuwmqp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3toknmvjh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3lqeadxnb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3jthixuml.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3sooecshv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3uehbpvgp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3dmcdmbbq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3mnhwuavj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cewkyuqj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ubdiidyn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3xwmroqex.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ceyvtppw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3vvfcitfc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3houplgfd.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3idxyaavp.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ghhigocm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3jixthveg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3mxhzkpcs.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3bghixtly.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3gzwmouns.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3wzrrcxdf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ngldkjvg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3rlpuzxxq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3sqmcalmo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3xynlywvo.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hdrmqgus.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3sgewtcck.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3hpdadifz.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3jeyqftdn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3sjatrcbv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3pdcvnyti.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3zlfauagl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3poqcqkeb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3cubthicn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3awphytik.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3xdzyitiy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3dofbckmj.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ezmpgdwk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3rgjttjnc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3mytaxwtm.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3damraoat.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3dxastpew.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3edgeiaqe.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3mepkkroe.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3msoayifx.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3apsadpbj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3rkgklarv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zcnhmyjn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3drmpdcdr.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3yenhjfde.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3zokstttx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3irrsazkl.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3hzynfypp.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3cvbswjbg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3tpwvymfd.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3bahfxnjz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3jghtbnou.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3mrnnullu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ayducclt.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3dpxilicr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3cmpkocgd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3bzrqhtqi.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xmkxoiqq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3qxujlbma.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mypapfwe.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3rszzcgby.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3jfmzurcj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ydvsnjon.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3sgdvztzl.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3dcrivbfp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3pyvywriy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3kqlhpxqv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3zyoarqip.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3anzmduxy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fjjviaao.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3zwbbmnhg.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3pvtorocw.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ahnoechp.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3dwxtyvgj.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3acxuawoa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbppuavb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3jlmtolwk.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3vepyihjz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3bkxhdoqp.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ntsqzqsb.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3tslcwucg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3jcswlqyv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lyctqngc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jliiuuzo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3pfjdnmsn.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3dmcbmuxn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3gqnbdcol.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3iiiptlaq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3elxbixjx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3sjqmdkpg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3bilwopri.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3azdbkwaf.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vfnjwxke.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3iqrzjqca.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3zujofemh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3xfexblnf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3jubtfpqu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3rkynbymw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3bjllyzhg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3iiejnoxw.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3atwxynfi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ujsuzcyf.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3phsrehvl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3sxnpnpom.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3sjfwbuzd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3szindpzh.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3daktdmjj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3cpqlnqgi.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ykoljlju.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rzdrwsxh.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3rkevqxck.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rqouivqi.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3luyxuequ.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3senzbtcl.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3orsciawv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ggnpbikb.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3tjbnwhma.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3snlaoujr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3lwontwrs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3rcoubpun.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hmthgpxj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3tipblpmt.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3jwwrzgwi.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3avmakpjj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mnwvjmmr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3iyhglsqq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ajsajxgi.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3oqcbhuie.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3sgfuefox.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3tgjkguom.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3spsymwfc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3hsfdnnfc.html


<!-- 参考信息 -->