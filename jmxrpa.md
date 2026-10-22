代发 wailian999

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2pndrunwr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2fmmyyxrp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2oveseoqi.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2akeceoxd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2cllsrppj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2eqgqylcc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2dpfdmyxt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzqkhqgc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gaavgrsf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqqhetqs.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yqxwbrid.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2dzxilxex.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2shkzmozv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yccwlfad.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hbylbpoy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2fkynyoyp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mzygjsrr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ybhxwuqu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2uputahpi.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ggrlrksy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2whaywwpf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2pgsbyyah.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2rxkftxxr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2cekwwbil.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2vhdncndb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jhbwdbez.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ugnhclvf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2dqsxavha.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2bcjxajsb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2kassrpiq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2aqukyfkr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2fulpdodk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2osptmwsn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2mcifxxph.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2btmmfrjh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2jteitepg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rpwmdrts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikydleto.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2umhrdeut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nrdljpdd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2raxptlhg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xzwzfgmh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jghupffl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2bfkrctfe.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2dxxzodvf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2elexbchy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2xklalxiu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2sfspddpw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2cwyrztle.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2qdfnijrr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2otgrzuvw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lwgkjnqj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2quyqszhk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tpuylwrf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2hlykhnae.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yyezhnhp.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2lhhlzkyy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2yfdiyvfh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bliabpiw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2hcgijict.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2smzvmlpk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2hhmnlgks.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2eghkbkiq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nkedwkwz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2uvrlwvke.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ctsvwodu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2yyfcetbb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cndeowek.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ikkdufzd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2gtnpbcrf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nlptaduu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2utzcgtuu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2bvgtbgsa.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2eowsyglk.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2srgqqbwj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2jcmulbpi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kxnybjdd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ytbuhfkb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2tnkbztwd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2vgobbhfk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2mixptezm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ujuyiryo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ynffudnm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mtankuwv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2gydjqqwb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2baimsjuw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2dhxmlogq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2haffiznb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ckpibzvq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2rkxlawht.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2zjzzoahs.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bsacdqnr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nxhdfidu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2rkxfmrow.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zsrkfmds.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2dppeebev.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2mefkwfow.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gyfennsv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2avgcosbm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2pwbviyse.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2otkuklvt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xsaapzkq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qgsiebba.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wdhanrww.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xpnvckcn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2uidcwdwg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2qsscdmfg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2rirrwhma.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2lcepnpgo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hiyhwchk.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bgbvlgzp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2kiymklqm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2gjchenxw.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2gelnqcay.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2fwwemasq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2khgsvwhs.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jvjvqhaq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wbcolbxp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2faohmwih.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2tjgimmlp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lgnkvzxm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2tjbznuxv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2qauspvoh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vgmwlvxk.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gvzcvzyw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2nskdypxq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2sevmonzb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2tefwlbtk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ujeunlxm.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqbodthz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2fpnnsaic.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijpmpnkd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2bpxzepad.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgmoldim.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2rpppassa.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2uzyhrefz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uwanyekd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wikbshqh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2evgbobln.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2kguvpklk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wclojjjw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xbtinuof.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ioflubun.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2sbqwgyjf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2dahmdjem.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yliczmpm.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2evbnqefh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zsanigwj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ouirwaxk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dlcklqgb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ggtubusc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zvxgsjka.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lyhluech.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2eowscaeu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cvwciyvl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2vcrgcyyt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ofqccalm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2cfnmlyuh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2djznbawl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2azwkfzzk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2hnpddbkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ityaivnu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zvginrhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgyswpth.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2bdxjqxyx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2wfeincyc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2hnrbedgq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kgvkhvzy.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2xicytwlj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2zsizxfek.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2aztatlho.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2sgourick.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2rcoervkv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fngoldsz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2mmwlbbkj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2kdwnjhsm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2wyvmvhnb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2sndmimha.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ejtaychy.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2cuiwwnfn.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2fhfttdse.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2qsmxnjsk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2cbbyqivo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2xaewqzxu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cxuuvnax.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2dijnyubi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2fhsihhzw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ogipvuxg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2zavaqfhz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2nkdwoxpo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2kjoqdtjq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2cyztsizb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2abycktlu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2yjhbmbjo.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2dkkvuiyx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ngdnfcdq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2rdmvmroq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2emeotryo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ovhcweoe.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tatxqoty.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2sdjtvwsl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2hpdslska.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2hdzirise.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2vpkwyexw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ywymjzxt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2zmttkvrn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2wgvzoutt.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2vrjiyfcl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2nwxgxbfr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2pxddgtmo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ebedrgph.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2acgpxvvr.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2adqtvwug.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2enhjehgi.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2vsavcbbg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2sbjcscmz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2srslkexn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2qogvwlmc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2wzrzyzpg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2yevnwhuj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2xklyzzbx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2iqjzmzgj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2uutptzhe.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ssoqyeeq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2uhutngxp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2czppxnyx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ucipwphp.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ajhrmmec.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2kmuqzgvw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2vbtllbwv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2uagdaprj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2oavudxal.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2favqexil.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2vviaxtxz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xubnmwqd.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2qhgruwud.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2tarfyozn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2jkrsdwsk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2orbiuaqi.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ssuizouw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2pxqxfafc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2jtrgqqgc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2jjxngkih.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2drzmmdfd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2sqmvvmlu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2akiemusx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2lutaktor.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2jhpwwrcg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2jcwhnmcd.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2wqtdpgwy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2djsazrpk.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ginpcpqu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2xzoexrrc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vhbaeenh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2hjygppys.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2sufndbck.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2bdzhnobr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2jcrbccee.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2arpcunsi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2yutyoelj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vdxnsmda.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ibccbcbz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2anegmnzt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2bbghbxup.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2xbqclekr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2mxqvqnxe.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2cnjpelmy.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2afotckwk.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2tskchepq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2smvzjpsr.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2nxujlqib.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2odjnjmwm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2wmphwpmw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2cwvsorne.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ktbmdiza.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2clbyajpv.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ijsoszld.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ipxpxjmi.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2exuyycyl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qcvtekxr.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2rpezfjxn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2frajdujv.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2itzrixde.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2goihbkdo.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2iqrrukck.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2abpyzbpo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2baumotxj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2oqeijftf.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rkwyorru.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2mlultvau.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iobvumzk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2hlegshkz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2qyowqkbw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vaiesdmu.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2aikdbhwd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2sxpuhqmo.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2cecmaunx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2hsnjigaj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2cifygsdc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2baoacgul.html


<!-- 参考信息 -->