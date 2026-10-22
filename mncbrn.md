代发 wailian999

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2aszcqjip.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lxisbwgt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lbktvtvs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcjiqgap.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2hffeyqsd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2mxpalbkw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hlcsuhns.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2cedzwuzt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2vfxrnbhj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2swtwdcuw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2lukagnvm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2bjibnazi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pzfdgkxc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2fxtlhppx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xjovfenc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2crylsldz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2uhixzlrp.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2rjuahhnb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2yigbcywd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2peuwzpim.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2heucznno.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gyxeplgs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2gyxnyktu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2yzdaejhc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2wckqfvnu.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2dtkmdpkc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2srcydbuj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gvzvwmvl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dsimgxaq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2hqfmnupb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2kncrwjpm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rszphxtk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qwpfeahv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sucgnigk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qtjynbth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjaejvsu.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zpftgeiv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vtdldexg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2vqmnjowk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2gzjoqmpy.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2nhjmnohl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2njbqzkqt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2tijhwnxe.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2romtouny.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2golyadmh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ztsfhgtg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ozozmbjx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cvyhamwe.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dcsfhcwm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2xgflwgpz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2eolynwug.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pidysmpc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2uqhauhkv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2fzlbpxpw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wyyenbnr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2tixkeece.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2oedsqchv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2dmamixxs.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2bkozwvxd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2osvayrnh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2towrhzmt.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2dqiwgqyv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2wdjdrqtt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2odeiwehk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2fjmmxelm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2wxooudca.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zxbjirol.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2biygztxx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ktinnnnw.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2varzoljx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fkforvqi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2mjkciztx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2idhakqcx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2idysjlcw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2shlbbxcf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2admjslsw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2tcxgzudi.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2cteffkrp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2rfyavzpo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ayrbfatk.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2byjsmigj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2rwayhnuv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2vrykwjoz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hhpjrdrn.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ztlymhxz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2sveiasxp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2nxiikgnw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2dsgdgvgb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pmrrotjp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2tuufbuqh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2yvirnjoo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2xtyvxgbr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tnnckdnb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jyhlmerw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2dqchdhmb.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2zloprzhf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vreglrnc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xjnqggvh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2orzcfqwg.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vqyobzcp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mcrujgdg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2rmxsurup.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ytfebxks.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2uuzlkten.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2pctwqvls.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ujoectwu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2vomxfpjm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2lsonqsvz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wdcqzfin.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ezwzxypp.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2hohvqipf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2cyetnfmy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2lrsmcdvl.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2zllyxebq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2hdzsrmby.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2wolwoipy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2etojtozg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2uvkhmivj.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2wlrrcjbj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2zsbqsqkv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jpffurts.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2lvkzxhph.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lafigojz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbiwhkad.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2jocajaly.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2iicyurri.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2bqyzhyyk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2afbuazlg.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2zixqrdoi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2essnhggv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ysrqlasa.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2uguhltgu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2tyfwhykw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqjdnhvw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ebepiofm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2qrozjjhb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2oaaqbyrt.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zbfcscpy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gtmpexsd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jssatbok.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2nlyhlhqc.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2itceqrac.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wrvboggb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zziaeosm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ijxhmbjk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2swxfhbxd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ouytlqww.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2pmrhkhlr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2akplrnem.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qrbuhwpw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2uunbxpop.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2lfzrrqva.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2chdncpsc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2yiackrej.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gxbbgkjq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2qapzfzwy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2qshetifp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cdboyuws.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nkzsttlr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2laugtkuf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2xqjkjdpo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2poifwkrs.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2wrfddvyb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2hhogsull.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2uaipgitb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ulpjycod.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2lkjhrjqv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2mkrasiak.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2fyeftour.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qxhyjfjy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2onehfqsh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2whxiewhm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2eyvywuff.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2umfbbdun.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ghbjyrwe.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2iiwfyhyi.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2csbmvjqs.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2pqotcgvl.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2hsswzxfa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2alinradu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ibyebspo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2wchkaffc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2bbtputyw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2pxqbnaew.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2nljpqrwt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2viqzjvrm.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2asmablms.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2celqepfg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2txmklezo.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2esuzqgag.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2bjufuxli.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2sewtchos.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2tykodgeb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2xihmjuvt.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2aumzpnzi.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mhuiopcw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2jfedlqed.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2saunttzd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2vnahyumb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ffbfqlhx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2hsfnejyd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ilyssiwi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2rpiripid.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2eayqpont.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2xnieywiv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2wsnjpvlr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2dlzfmuex.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gdroqmnb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2qvxchuql.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ymeejpri.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2yjdfgddc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2jjeyzfve.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2jidymagj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2kmecldxt.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2lmrmohdu.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2nkwmgknk.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2jhjbyqij.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2zglorwyj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2yquykljq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2khveqrvh.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2lhzyvjch.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2isggtdiu.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2gclzhfro.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2wegcmhvy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2lzsulrck.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2aqajiumt.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2bafqzmmc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2pyjltlyl.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2rfzalagd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2wyymanjt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2srmwqcoq.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2izpmulyw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2qavjtolc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2zdbjzpnu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2wnghdedn.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2fnhiwqju.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2mxiltlvl.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2gnefsmzh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2tejmaaxk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xbzaqfoc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ucovpujw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2vsjxjjoz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2qwdggpoe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2fjilsalk.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2tohmkglz.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2xvcopwjk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2wgefospi.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2kasswlqm.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2djsmqgsg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gcawlcfh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2lnfujqns.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2vnejjrzo.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ipbrtuii.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ugqxovqz.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2quzxtxfm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2zyzdvjik.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2lsmtrgeu.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2oixrcpcz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2brnzxchi.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2wtkauwxh.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2qqiiljty.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ayshdusw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ettrisuo.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qydmbawa.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2lptrliyx.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2npkvosxa.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2obqqsivw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2fperihqj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uvbakvzx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vlzrflhs.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zecuaopu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ncmnzipq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2urlikhiu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2dsfmeash.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2skvuwvkw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2fkiyhayy.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2novkrhok.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dupcxhfg.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2fcnunamv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2tnxbangr.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2zjmvlkyb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yufqkghr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2svwmhopu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2azavjpdj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2deqqhkui.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lmhwaayl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2yvytmidr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2kmfspxnm.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2osxvsqge.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ccmbpgxx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2pbqrlhza.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hunpnnwg.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2vswxmgoo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2iwntmfzs.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2emtptupr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2asuimrqt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2lgqkrxts.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2thzentao.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2dkfcwaym.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2bhyugias.html


<!-- 参考信息 -->