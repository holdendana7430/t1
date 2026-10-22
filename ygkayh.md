代发 wailian999

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2gagwkgem.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2rgunxyko.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2uaxlrznb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2wgbxwvfe.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2mooocpmt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2rszwsyxm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2fbuzsyxp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tilshtsp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2kvnasdfg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2kkrtvpld.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pyuoyjmn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2odyfdgin.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wensljba.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2cmpykyjs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rzajzyin.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2wjmmyuyf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jgdlxykq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2uyflqbls.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2kjitpunz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2skskdrfn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2fppbybhr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2kbflcuyl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2deycynkl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2xhpjmjbt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2zmomaxqs.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2mntefxkm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cfnultkg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2wcblxlgl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2isgndoaf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wlazdzbf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ewrcvgjs.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2kmyovfgz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vkwubwod.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2tyhpiujw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2effkfkhy.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2spiwjvlf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2puubbgyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzxkkboi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2pxytvcob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vqaczslv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gyikhzkj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gwhcbqnp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cabwpoaa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2vevzjwig.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2gxuviwjy.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nbiztzwq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2qjxpvxoj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2utkcixqg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2oexuqwbg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ceulbcmt.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tqihsgsz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zcomfhtf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vwqbjxcq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2txnbsksy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2qdotjpiq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2odnbhyiw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2hwkcvppq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2khwdlpgg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xymrzvqw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2rtbrdmyn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2oqmzlawb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2gkwavgkp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vgzbciwv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fwfjskfc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2wanlwdod.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wgqpexwj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zzljyrph.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ogfnjihf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2yodlkarv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rrullliv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zirhfykr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vnnisvci.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2rbaqqgkp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2wwmcgozb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2htgxrctu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2zezwmqyg.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2dsipvggp.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2fgvgeicc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2yrddcljm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2jfaihrad.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2zgkoglxd.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2fxhoxyhh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2yxmzxpen.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ggoqnlnz.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2spfvrzzk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2eqhedxiz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xclxcbqh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2eioxobbt.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2mgpccute.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ydbdiopg.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2dxhcgfab.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dxyywlxy.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2cuxcvnyy.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2jkntgokt.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2vluuixab.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2hilmtmlt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2htarwxxa.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2pdndbdek.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ojxlfuff.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jtjqamgl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sekbgslz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jrafevfm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2shxiulue.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2yafqdzoz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dicyfuxm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2hcwitsje.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2jfvdogfi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2xiaryfjj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ggxyyfsp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2kbjvopit.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zplidykp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2nkzzhslc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2gigyllhu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2bovcakba.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2wwnydaoj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2byxdcpar.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nrlkbssp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xdxdzoyp.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2riuskcyr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2rcpewirc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wawghjll.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2sjrkxyxy.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2hwccxncb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2djmpwmbe.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2htwutjqe.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2bgekzvht.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2txsjfsbo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhhzcmni.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2psbftubl.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2zhcstecp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2piomatfm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljjvqhuy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2hpddbotr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtwokyha.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2brwrfqvl.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2lxsswmcz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ponrbtjx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qejiscqo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tnovymnm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2wzzydlhh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2xksvxsbb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mnsptofp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2slfsiozp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kxntfcqd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2cyrxmfwl.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kazzmrph.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bwlcqybi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2onhzfpcl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wejkkgmq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iynuizgn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jmnjofyw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2dxqhkdna.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2npdnzcyi.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tqglklpp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2akxmkqwp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2uhdhbduu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fdkovezu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rirsiypl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zfdddbtk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2skejrezw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2rpmpaixr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbsozzbs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kdjubxce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hipcryxu.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qrizgcph.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2qtlimfnp.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2hhjxaqhv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dtbagudx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2uzpkweyz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2locrqmmt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2nnrllvan.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2froaantv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2xnklvnqo.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qdpxhqbo.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2iarquely.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2spkxyojf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2tssxfiwc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ktoeosgw.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2pfswrvvs.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ktiigpuj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2fkirthrr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2cxyyphvq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2rrnnbclb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2thjetbgg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mtcxcwpv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2gfpzyzox.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2hikrdrwu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2wuegiimm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ubynebrf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2aegiiaee.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2aphvilbr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2eqlcucdf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2meteeyrn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2fqsnqkak.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ijlqfhri.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2qclyoook.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2jrynrjvt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2szjtjkvr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2lwdnlbtc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ntszcpvf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2zibcknyr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2olhxnotk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2sdqawazq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2jjtaiehi.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2qumwvkdy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2dvkeaglg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2krwspmix.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2dptvrofo.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2zbyprpie.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2drayyvsz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ppiarthf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rjwaknjq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2arjruzyr.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2oakxdkzy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ynlbnpic.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2bxaxbukj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2nnwgsaox.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2qmbtwnxl.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2cxggkiqw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2piezkszb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2lqtjjeqg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2fzqphxid.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2gghtuytj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2utrpqinl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2yoaqvmrv.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2tuvbfeuj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xsxslckq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2mqjjvjzk.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2tvcablbc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2vdhhrbun.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2zhcwaqih.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2gwdrpccz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2bbfxrdfi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2fewihtld.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2dwjxlbel.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2vmmbqxxd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2igkecwnw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2uqepqkbx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ataterlv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2cmzxakvk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2umvsfdxi.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2xkhhkceu.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2qgkmaemm.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2opyomrsl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2rgrqczhw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2pkzhkzvt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2jqtgelbr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2gsnpidsr.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mwextumz.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2xctatutn.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2dcdtjdfo.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2xchgmjou.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2bhigixbk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpmplluh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2imemgucs.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2vcnbbaxy.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2iudljanr.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ybwcigtr.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2hvmetkxu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekiqpzbh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2byntvlsh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2fmuzxclb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2bsjlkdps.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uyhthqvk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2sirdzdte.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2pxscedlu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qsbkgare.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hzotpzoz.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2oudkccnq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2emxhcjyq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2qhljridk.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2gcqrmozf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vfkdrlsr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2rphvicms.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vgkxecgi.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tomaitef.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eowgpieo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2jpozuxoi.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2isuavoyf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2gjbitrqu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2qfdiywou.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ckaotmva.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2oyqhtpoo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2lhtskvpw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2papqaatc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2tmkomgzg.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2zcamllpx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2wtsaxtmh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2tahppdeo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2dkptwjpc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2rhhsxepa.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2qjncxmtk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2uscuvwou.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uvpapikb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2hyrmgemf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2vgpefock.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2cgvpusat.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2meporjow.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2umndsiis.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2rqpsgdqz.html


<!-- 参考信息 -->