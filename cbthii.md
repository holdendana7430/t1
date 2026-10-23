代发 wailian999

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3vqmqwizk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3pnkncmlu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3uedxyizl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3wfqqxlvy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ndevcjvo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3pdllqimr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zsgoomfk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3fxakeaed.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3niajbnqu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wpmvpkyj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cljtcyru.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3tpdccjjq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ikbdfskk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rxslwcao.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ydzgqaib.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bsgajeiq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3autjvwgk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ehihtnzi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xurjbapd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3qiepcgdr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3epcxwoeq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3kfwbuaqs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3lgpmgxvy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3imlicatj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwbemclp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3akzbdxle.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fewawudn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3odzebqib.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wajozwxj.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3vqqhqwaw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3udjopfff.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ossyhfva.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3evzpcujv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jyetsmos.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zeuppujo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3teqdzchz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aownfvwb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ybjrbchb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yhijhviv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3qskxhbmh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3nyonescn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pertohdp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3mphtbklc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3deeimtfp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ogtiyblv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3yalmjjfm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ejoomeis.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zgywhnxx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dqxsiopu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3iicpqyfi.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3vccpisrg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3scluzvyi.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3nzwsvjcc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3blstgzix.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3gsdqowcw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3zjqyutce.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3mtizxbco.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3qkuutfxc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ovofkexh.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dlolttjp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ekyhezcn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtedbctw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3mvtqoczw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bkhamcwo.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ucdkmlhd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3mkebhtfi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hyutaaco.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eyfvaeca.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3cnplizxs.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3llznlzft.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3btwaoewm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3nshrwrfj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3hklibehl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3vxdfcmfb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3kxfagjnu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mxsijamk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3elllndro.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3uppslsfm.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3inlksdfp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3hurgqfbq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cmcokloe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ynsjames.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lsbuuudv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oahmeyea.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3jhiwhgxk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3wujgzpor.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3jgosgjuw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ehoexpap.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gbwymwhz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3jfmppeba.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yficcytj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3hyirvppg.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3sywapcys.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qjouxpnr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3qfhremva.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wngyqleb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zpbxhfsd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3giuvflmi.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3gwsbqxgz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3lgmezvkz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ayvxntpw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ipgfjurj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3kfovgeoc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3bmabctpn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3wpdgnixm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3cqxjlcvb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3nqdvzhdt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3byrcdjol.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3csldqacf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3fotirxla.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3guzaphzr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3pczezslb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qhzgvhqn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nsurbiyy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3fzozhdrh.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3rvaumvlt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ffkhpseq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dedhxiqr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ieglstfr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bjfryxbx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3queajcov.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3sbfwjhjz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3lrvtahjn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3meucrqqr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hugmjuht.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3lpeaxbsf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3qeahwtnz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3tqymqkev.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3bwfssprg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpyiczac.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3svblezkk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3cpsvupvk.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zxhmrhbr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xqrlgzho.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mxmfgldj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3pkdnzjms.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3klchldym.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wzzfhvsv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ypdcvrba.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3kjexenms.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ybkzyaiw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sgqpcszw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fowrrqgf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3oromdcha.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qxkfcowp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mmogzobq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3iuaohybj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3pjjjcrux.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ccybokgx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bmrgcvtb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3cjmcrwxr.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3kqeapcds.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3xjxiwghr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tjoqxkcp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hxsqxzzw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3fgkmysfa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3aaiwlnrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wzllpyaf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3twlesjlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfyvnuuw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3axnrbusz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3dirdpisy.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3rvzszhdx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ewnfteaf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3urvppulm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3utxhchyy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3rmqvmtlz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3hcdlqyba.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3pchfkkut.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uxvrpkuh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3cajynjrf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3vjvmcfjh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3kjutkmcm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3itdfwrza.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3qerytrzz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3cyrvwgok.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3biwlxhbo.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3gtbdrolj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3hwyvlmhj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3fqgyestw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vjchajev.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3twtjwyvn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3qknvufbo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cleqfomd.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3eyxtcozo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kgnuwkzk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3wtzuksoo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3mcbfcdcg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3lxkxxrdb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3sjxtbtmy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3agnlmgmb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3uwjrmyyh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3uafqfikd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3rsfvixvz.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3gbovvxbr.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3rstyhlzl.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xuxzskkr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3fmaubgjc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3jrddscfp.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3jywlgxnu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qgjwzzdb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3fctvcbwz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3euoqggqs.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3qwqqdvrl.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3dhpxrywh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3mdvrnmqc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3vafboylp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dktocrco.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3gdsxgxdw.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3siuzjftj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ssevornl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3dckctgej.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ugrvzude.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3mmkftyvm.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3izvcyjbj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3otcfgxlb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3cmgvbntk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3jfytxlif.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ufapvsyr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xafyrkdq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3fcelkxae.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3inxijxhf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dmqbdazi.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ktjcqyqc.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3bwxgtisl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3nigmglvq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3euooyhdy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3wtplyfia.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3gemybnpm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3tfvkezba.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3xiteuzib.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3bldrpssd.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3uqwkqhcs.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3lcsqknqx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3nqaqvexo.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3mcqpiryp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3gexwnvbk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3wssfqedb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3xwnmzzhd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vinjsgbt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3znfshdjl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3dcxtxkzj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3lqfpxmhu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ydazldki.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ppoiregy.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3vtputdth.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vpmsjyqk.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3svwxdxeb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3hprcxsxe.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgowuhsc.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3dhoaxiti.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3hznlgcgy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3lgmsdhpa.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3gtwefrmi.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3kezpecpk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3hktizdqg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3uzmgnoga.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ldbpdmmb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3kfdgznvu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3joltayji.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3vpvxriko.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3jwsmgujo.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dyugjqyz.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jwqrtftl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3eaimnlpn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ryuzruxc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3whmhvyis.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3yckvrxiv.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3mzrqvedm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ejfqjfhw.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xelxtite.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3djjuywih.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vmgtpxni.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3dicvhbcp.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3rvmwcvkv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bvipisug.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3gpzofaqn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ahmbpgqw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ngkwanut.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3crijvdhj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3azjskxji.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zdlxyxii.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3rpigamxe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3cnhreimt.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3wxupbaxr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3bdfjiukv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3rqxoufaf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3hdbvgvmx.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3hazjxxjc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hvuxllki.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3kolqojpw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3izzmzmqz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3lkwhokju.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ovsaavns.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3mxqzipno.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3cftmanzp.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3etcjhjev.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3szdolqsz.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3alhduhhc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3cqkvbysg.html


<!-- 参考信息 -->