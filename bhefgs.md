代发 wailian999

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2iwzzphky.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bkcliqqr.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2yhlbzvgj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2aacqjftc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zszmmohv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ucchvwpd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ctzxqxrz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ixhmrshc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2egqkhwqw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2fcnqgbsk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tfgzcaze.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2slrpjvmg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ddogmnea.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ahtcerfu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2nedltuoy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2mdpwlnhs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wohljgqs.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2pvhaljex.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xuizbcip.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2smvsdofa.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2fcrlqhpt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2evvegepi.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2jvsnegml.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ykauojou.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2debqaffp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2etoopauz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bzgcclbh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2bmifypny.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2grgicjsw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2cawxxyub.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2myjqehbf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2iczvydwn.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eqnvonka.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2bvlsijwa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2sskhqhux.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xodvjtfl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ugtzlnzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hrgsyego.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2umwchhiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qqlhlgwb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2aqdgecaz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qxwqavja.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2qqbsmqan.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ilzekfqh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2sqgwfmrj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kpvliurq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2tlhnjhas.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2cbrfxyct.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2vuybzhfj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2sfoxgjix.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lqulfxmr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hynzedwp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bittjpqi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ecchtfxb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nsstkkie.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2etnawhzy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ecsgdxlg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2faduurwx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2qixktsuc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2suksqkke.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ljjvvkfp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2hutnjhfe.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2zatahwug.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2eagbpwmo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2faannzsp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cptgiisx.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2dggxayat.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qapjtfgs.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2vorxuygu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2eovmewww.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2thpougoh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wnywyikp.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2lfpkrcdy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lhxmsxnw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mgkgzbzq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2cuzfmydd.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2oxgsgwgo.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2myycvxsg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2miqxiupg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ezqqdbao.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ukedwwki.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2bucsprwj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2paibqhei.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2wqyzkfzh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2tyycjesv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2pxeaogsq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2aujtnyrh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kvjpxtns.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2eivntcar.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vlfwuprp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2vjhqpxlp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ycvckvbw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2umhvmcaa.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2xivrgtxp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2gapjzctx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2taevlvai.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ybgzsudd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bxqysajg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2dcnjvpsl.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2wedxiria.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qbkneeoq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jifqgrwc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wkyabxrd.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2bqmyxoxj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2mwrzuovy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ghifmmjo.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2qboleupa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2jbnlztup.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2jvgxismr.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2hdjvayfo.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rigdsxsq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2dsdwmjko.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rjpjcvkt.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2hkfdittj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2nbssqucl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2lsfgtnav.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2guaebcur.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2zajixzmv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2bfblvkte.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vfmoqwrn.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bzvgfgzf.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2etmsdlrr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2pqiwqmyx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uslnvlls.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uqsumazb.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2txjyzozn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2yckpkmer.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkhpgcgv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qhnjawbl.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2qnsaqrwz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2bjwplaml.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvxvrjqh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2eziaudmm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2xemggcxs.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ybqgmvbp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2aadiqdsy.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bnrqfezd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wtvmhzgf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xrvlwhuj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ttedetpi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejjudrei.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aysvlrju.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qqotlfgl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2jswmqbot.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2qakjkbhw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2folcaqnb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xkjgzmhv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2exicirhz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2obiqjqai.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ftltysuc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2wbmtimyz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2qkgazywc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fegxfgal.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yduufzja.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2iiceibyy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2oigpskpb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ogchlnpi.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vcylhlyx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fzjbibnj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2niwqxnql.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2unwzpmfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmqcplmd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mgqkdcyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wpxbtajj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2mghrures.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2cafvqmcp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2uacaccle.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ffeotfxx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2fvfitutm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2fdkiydzp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2fybomgjm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2agzjexpr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2bahephbb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gozczpcf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ztezworz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2gvnwczts.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kcumzzip.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2uqprburt.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ahwjjcvk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2kbwjhlva.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2dogatkjc.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ckswxsgh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2elbcligs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ryhyuspd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cpaohjoq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mfnjuppf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2sevaqutg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bcsumzzf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2dptvqezu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ddrbuyco.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2sbmcmdfu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2gyqugfwk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2satoohve.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2zonvbhyq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2frngvvil.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2qedakbse.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2jpvvkaqa.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2nsxzvlwx.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2kbvomldf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2hqqyjtmg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2nefmjhqj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2zjsgvlzx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2prqucyxv.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2tslznqmg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2pyszhkdx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2dyrfynie.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ebjetqch.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2hqeisihe.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2kqptiyjf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2uvfiihcl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qyiiwbhj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2smdhmxmq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2oemcmqyq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2rbtykvrh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2itmspqia.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2smxxfdnx.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2lzkvpsal.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ttoqlpir.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2zikpmxqu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2krjigxsl.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2kkajgyre.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2kyoythii.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qkynonjm.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xpdhnycy.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2oejqltaf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2geprtgew.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2goawpbfq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2yuuqhvsh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ylcbhqfe.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2iufeefrd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2qpsgydhm.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2xkagwuna.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ebexnmrq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2gkqzrihf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qnzmwbqs.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2zvyhyrkx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2kehqfped.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2wfaucdxy.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2gmtddcnj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2afjcajjt.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ofiitwhq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2nuiuvugu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2iobtcceb.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2icdtrhir.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2okcojpjv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2mrsfodaq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2junpsgto.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2eounsnao.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gnpbwxpi.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2nbrpcgqg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2szegidfz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2zmqqxuly.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2vmukwzbc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sdqufmia.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2aeemopyn.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2dhchtukf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2siyzwoko.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2elkxjuyu.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kjkhvxtf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdqddxqg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2bvclddtw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2nxzttbcs.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2fhrrautf.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2yafunhdw.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ykzgduxf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2mrzazhjq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2eizftwkg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2renengfo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jaurvqav.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2rnvmqxdu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2jvgozkdc.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2exjoyzyv.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yzfgiyef.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2opeufqqs.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2digqtykh.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mzuvjqag.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mmfzulgl.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2rrdtapvy.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2djogehjb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2cxouvtux.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2aeqpdvbr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vzguabfr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2wwmwxkeu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2prqwtzkz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2dzqbedbf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jgynjtxm.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2sgbqmhml.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2jevdzbgn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2jnhzfxoz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2gagecvtr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ajbqjmgn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2eflonugb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2dmzglvli.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2optenbvx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2xbmcctgp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2cnpsdkzz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2vfmqfyjq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2nicsxmda.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2bxthcsno.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2qoqocnch.html


<!-- 参考信息 -->