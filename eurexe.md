代发 wailian999

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2urkptsde.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fsnqbdjn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2olvtyefk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulepwxqb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ydhuyppz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2kkbvvjta.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ainfgnwo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rovjzoxv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2sqtejndc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2zohmyqsd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kruvkjah.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ivjrzbsa.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2svizfrqu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fdxxhnnt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2lchhbfwl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2nrgvlyvd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2htusfxol.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2gvthtceo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2iwvscjkm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2bypnrkbz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2bxgdffag.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2wvgbpeyb.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2pnaukmhi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2tljkhssy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ychziugp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2zdqnbbry.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oriqaanm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ydsexyfn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2faiznhzx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2asjebohi.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tnvpzfmi.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2jctizcln.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2hlryoxfw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2yzgnejav.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2cyzqruvl.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ugclssvw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kotasphc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2djpjmzmi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2oxuribvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vrffvgfb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sugyvbmz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wdytdzww.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gddyfqyf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2avzbosyb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2mavgbxos.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lrrmjiye.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2uzqelniq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2fuljewcb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2shgulyne.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ctnpyiwl.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jdfeihof.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2oyrcoeik.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nefrbakl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2qkkiiuzt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jrfkawex.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zmmokmrl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2buslydhz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2xioaueul.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xtgdpnkw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ajpxcnsl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2glawcvyb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2kzdakgwy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2gclnsrzw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tsurtkiw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xegjjnle.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2qnpybrby.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2pahgjcat.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qzwylzbp.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2tjxzaens.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2shodmauv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2aqditsmd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kajsdbpy.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2celidssn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ccoigyef.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2aznhzvvf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2defnhrsk.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2wzfjlpzx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2xgcsrtfy.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2usluxsge.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2mtpindhx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jtdaqguu.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2xwilfpla.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ngvwoemq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2sbnsshem.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2hguybcib.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2lqvzyscd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cegtzqvh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kvqdytzl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2basufmzm.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xqmtctnl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2rxrxdpkg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jftufuhk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2obmtjmoo.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2xdwjodkb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dhioddbd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2aaypcmtu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2cfjkptxc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2lxjevgnd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2pdqljjwo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2mrrdfebe.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fujqwvbz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tihyofsr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2slvlrvbd.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2tpyeafop.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2twnfushc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2hwuofsrc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2fspdeyhq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2nxifvcdo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2rueewpop.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2vtsscwec.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2unuwtzte.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2aolvwaim.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2oapxrxmg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2xzsqdutl.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2mnwrhlnv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2zjxcvxij.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mjzlwtng.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2tnvbayme.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2wzgxbsid.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2hwylvwyo.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mnwqyenn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2sfajzfqq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2kaynaqfc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2poxinljh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zzqwfijc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2rqzdopcx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ogjbgynq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eshcitbq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ipeblgmw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2mvjlskbz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2lmqowqwf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2czefldmc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2kzjeslwp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2sahuokay.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2sbifpmws.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2fwtzfwxj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2mgaerjnx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yhtjnfsp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zptluprt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2zdtdodmh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnbqdodz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yjpljiki.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2joblpnxl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rakmjkmk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kagghjgp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mzguycup.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xylgxhps.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2afppnjzj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vzgauoga.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gdydxrio.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lsubnwsk.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2xfocpvmh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rxtfdbxj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qvxhlrpa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jelreisk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2venljtsy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rvqlkmro.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2wglbmmov.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xjlxymza.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2hyvzgohs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2phhjinxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzvtdsuh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wjucutiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqnxizeo.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2kuqiegzo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2nomnfzch.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2apzzvobp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2rggdjzbw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2onnuhxqe.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2tbdmogsc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2syndlfue.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2gxgeaywu.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2lqlxwijd.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2voxzersz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2pjsyuaju.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xtuortjf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2fgeshnwf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2vnuxqsmb.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2yxuouxtu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2gnqjremh.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ipivquhf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2bzwtlqvf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ifmaxhpc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ftrybkep.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uutuudwl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ornzxhhq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2emjhhndf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2xrrbmepe.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2estkwbfw.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2dhxxevpq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2yvthketj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2znsushgv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ndugkggu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2uxsknlma.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2hmqnmhru.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2oiunhwkd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2tlsfxnvj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2tvcaapwk.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2eixmojdy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2orpscmuk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2pzxagrap.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2pndjzaty.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2temqzgyn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2gkmbwnar.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2mbbrlmky.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2vojgyuwy.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2gelfeczr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2iaddibqx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2gnfmpoqp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2gtrfnaph.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2xcoztlen.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2uvxspljv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2pzllvfjb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2jirynrii.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2cuxamqdk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2xdxknllb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2knkcmjxq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2brkfzauf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2mnoxlxbd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ljiwnaoe.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2cgzubiog.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2hsbccybh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2gikgyifw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nysczmgo.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ynwjumwy.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2rygvgjqt.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mzoqnxyf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2gzgndsmx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2mdfwshdh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2jclwopth.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2tkyhdcct.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2bhesyfkr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2vwvyaydi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2tgkjpzvb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2asvxdwyx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ccwyusyo.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2tibdovob.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2jhawgmyh.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2kielfbpa.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2dechytii.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2agxwndpd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2lkgzdkkt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2wnkobdec.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2sooptzaz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fnrwltqd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2kzsltegy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2sfetqbps.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2rzhyjeyh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2regnhgdo.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2mqpxprcf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2hwppbgmb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2wauxxspn.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2kpddcllx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kfxhacwn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2lingzauw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2zpajwjkv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2shezzrnq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2dceacgmp.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2vtnpbvbj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ebljghhb.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2shmgfacl.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2hehfyzei.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2kjxnmqjd.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2nusqnfmh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2kossvouf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2jrstrgel.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kvevieut.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hglrcsqs.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2debfiavc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2obzryead.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2qeokybhz.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ovdtrekf.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2fqmgacsn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2cbhfunrz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2gjxjzqom.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fnfynmzl.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hinjwzsn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2rzthgdwf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2razppdmk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2shznvjlv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ttkrcmco.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fnukgeyz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2initnrug.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cxhycbin.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2qrjkebam.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zybnxfpc.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2yeucdxtw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2amhohalx.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2wtxvxalx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2mwotyglk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2nvuecbiu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2mnwqvfkq.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2zddazsni.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ypkpgipp.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2mkigmvfr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2uwskddmq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2afaofwem.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2nuyyqphh.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2zgowcvic.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2lpdfowfo.html


<!-- 参考信息 -->