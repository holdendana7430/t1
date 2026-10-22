代发 wailian999

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2qdgmaqmb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hoofbgmz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2lfmhxowi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lptifapx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2lyqubgyt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ckdkgfte.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2leoccryd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nijqcssk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2shasbqjr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjcatcgz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yakzfbmy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2axhkibjh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mgifywez.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2owuuabgz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xletcyzn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2wcihsxim.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lokptalu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tihylkvc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2wzainyqh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2eckfrscc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zfwgkqve.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2uvhdzwcw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2gaoulzgg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ujmemsov.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2tpqzjpsn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2zbqnyymc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bjsbkuki.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2tlgnaedy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2hybkmtay.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2yllbtwxp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2gxsqgags.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dicqruij.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ooxmuvcg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2mwltunwo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2pnsyybcs.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2nixdisqm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wcdpbmdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bscjnxex.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2uaezpixj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jixqawrx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2okrmmvbw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kdvvfkfe.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2hsvrnitu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2gilcoorc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2gkrxpkml.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fstzgwub.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2snegkvbd.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jnvtrqjp.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2rubksujq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2hpigyuup.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tkxeodmh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nxkihmai.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2orgvnvhz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2bdsmewqc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2zgrxbemk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2aweriyqg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2vzfcffeb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2epyhagyn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ooemgnrs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2sqrdwwlt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2hnwxghrp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2mrfxpywk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ytwstdsr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2blakjotk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2icnprlwz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ysnupljm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ehlqrsba.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2crqxfkpq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2oilxatii.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2tmubrdjs.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yjfbtkyf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2monjlvpb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2rdxhdcak.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2wxwnojch.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qbziqamo.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2sksnhwij.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2lotmhtsp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2zpxawntf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2oafrqzhd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2majzrgcy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hykopyga.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2fpfryvcz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2gdpwfhib.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2rvaucljg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2pedvramv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pvkzdyyi.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2atqopbam.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qasqhfnt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2wcvhasvu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vugwscar.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2bnojcjku.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ruvucurp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2odjqbhrw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2gwrmuejw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2inesneak.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2uqabkwjm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wsclrkul.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2hbcyhzxs.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2vzjqasai.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2bifnjgzv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ldlzyylu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2iihxrkgq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2rgnrbsve.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2rvwtrfec.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2vvafrszq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2khcxulin.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2gqkegptz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ujzupvjb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2nmpyxswk.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qutmwrsh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2hkmnsuzx.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2vmywsvya.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mlsfslrs.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2sijrhbiq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2qaxzbntt.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2aeoicghz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bvafbcnx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2blmessyd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ulqipesb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ctvvhjii.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zjbewabt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2srdxjbxb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2sazrmjzd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ussmjksa.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ztwtfcij.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ogpgcsey.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kwakqizg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2rmqyfxjz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jbkdafvy.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2qjxsrzay.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2mvvrgmlg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2xvbeesua.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2twnuxaiw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2pixltjmg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ndpavydo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ilbsxkdg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ouebyoer.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vibcfjce.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kjilusqg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2zusqoheo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2fmeeuoak.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mqgpkjfe.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2evllxkpb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ondgieai.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2fjratwpp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2caxhzgdp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xoibdspz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bgtdtlpl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oliloogp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2uwswqaiu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2gnwovkwi.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2rxfxljms.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dennwlqt.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lwmvuxyx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xzxdydcd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2gbhuzlre.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2smylczxf.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cmxhspqk.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bhftutuj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2wgeuamsa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2zllllcfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dlxabqze.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2dlubzoer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvdvhqae.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2udxxrykg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2kxsvxwqb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2oglimgbq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wjvuwvju.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hllcaafc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2wggpoqyf.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2tqastyxd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2mojpfige.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ecqwytke.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2utrfgpqz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2pupuobir.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2fxcyevau.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2zxvmoaqc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2cgxvanab.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2axvswtyl.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2nabmpaep.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2gtaylzxj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2sphsfutk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2doajthix.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2jygqbzlr.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2kpjsjgeq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2nqzegkyc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2mkdzvber.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2mqunarvn.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2nxhmppgq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2zqjvfnfl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ilibphfq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2iovowqbp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jdlcswoy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2cseiqzca.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2pdagfjcb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2jjedpxtp.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2esbsmrby.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2qgxtlwox.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2bcjupygg.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vfinktox.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2jwgwwkgn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2lbfljztb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2nqhadhpj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2sqrgrgrg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2tfcwrtch.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2gjgyqwlc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ugvofpop.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2qbuogtjz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2qpwelxnh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2bndxxlqz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2fhxciqgx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ychutece.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2cifnkajv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2nkzdwgsj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2kglcedog.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2xbejbpde.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2yxpcgtfz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2kyqdtkwm.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2vgelxvky.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2eetgkqjl.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2npajnjxf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2acgtbcpj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2vvchjeze.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2hswngppy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2tscivvur.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2itibwgql.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2khobsspw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2gzarigcj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2jjghpkzn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2bmkozcia.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2pidcyxyi.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2izhqrrkw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2xofltcpw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2gyhsjjvz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cfwgwtjc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2vvvxfdbv.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2vnjavygg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2eoomgeih.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2thhpqjjh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2hwmtjznc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2duwadcxm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2qytiubek.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2qsmtfnbn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2pmefihpo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2dpjhoggw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2cbtgeuom.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2woyhujzo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2upjezkbu.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2awokyyrm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vsyjrhrz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2vfylvcdo.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2fhldunwx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ocvdsojf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ooelwzke.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2photjniv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2tbipjfti.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2maaapnwr.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2onaslfja.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qsxigixy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zflczbvg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ztagxbua.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2exgrnxqr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2nfdvzjwm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tumhbutg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2unrivmdq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2mztdgveq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2petpaywa.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ixclmojj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2tpvuafpw.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2aqsbtgwq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2thmfniul.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2edrsvghq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2mkiuyzqp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2nvyrzjsh.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2dxrkjpqh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gqytuili.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bwrpiwbx.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2uwjomczc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2sxykvdrv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2sovlykjm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2lyzpifon.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fxoewfsr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2umrteoow.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sicaaqcr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2tucjyjfl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fgflimqh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2birdnvme.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2wegvgnds.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2bpjknfny.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2cqjxwjoj.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dfdobzmh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2sjpylhwg.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2orgdkumr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2iwddqrzs.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2cwrxepzj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2llxkyvdm.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2pageqedz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2vhzeeefu.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2jtindtpn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ksnwagzu.html


<!-- 参考信息 -->