代发 wailian999

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2dmjiwiom.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2isleqaur.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2umrqqdko.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2oxtfddfd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xymwrdgh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2bhadzvzb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2jepuwuvi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2kqafgsdu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2njoudtdw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhiyxqoz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2blcyfxhi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2txvjhazl.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2eaxwmlmy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zpbqsqqb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ytpucovi.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2mfbxsgmz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tvasmbee.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pmqyrhod.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2wbkypovk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2tpmrrhef.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2oadwrdfv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2bzxezyfy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2evmbdxlw.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2rzmqgrwg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2vpfjvubi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2siobbyke.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rpelxmxo.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2hnxrxlry.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2axkkkkcw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2pxqhlval.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ssdwlaxu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2oqomhwpj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2iidpeebb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2scbxcuoy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2jhwktdng.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2urctrxjj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xkmtdgqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ksbmvxca.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2oqmqterz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hohkocis.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uhkvrdhy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sndnvhrf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2uqpgepke.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2utdvcmdh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wbbcxlxf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2akegvdko.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2xoyyyaws.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wahquvgl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2kquwfvlb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2shushofo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ofjpzpxu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2aetskocd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ogqdzghf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dqtofnxl.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jqwjqoyq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ksryrztk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2znbefter.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2oxnjpcai.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2jhosknau.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2phmdbxlt.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2kwzoedol.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2rdimrpwz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2yxsdwwrf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iytcvyrj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2crbssqkk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ssacuucc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2juojdlpy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bafhzptw.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2cisyilyw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wzmgkoab.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2irbopner.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2reekufyo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2lhlyvdtl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hzwpthzv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pjglmhvn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ozacbqbp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2zswabycw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2aregirwl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2uucbxvpq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cyhjqmjg.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2alzktmwf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2clpkrttl.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2klogebnl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2czuxvdjn.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rjxpjtgi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mpvvwwqo.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2aecqctak.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mfitdnqq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ctqpvqct.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ksdinilp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2athzwtyt.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zxzimbpv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jtmctpia.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2xoqjqapz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ofwvqttp.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2qtwtsqmp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ocxicqib.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2suzelkfv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2wguctqyi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2xfsdptnl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vdhmtlxf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lnweoqem.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2gfeshbrt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jutuzaii.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2dsusvjap.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2jypmutbs.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2gmqjeqwa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2tmxqfsoe.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2imdxwmbb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uaqglgwe.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pizgexba.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2xndvgant.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2stxzknwd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2mmnwyqke.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ocyxdujq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2zgefhfny.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dmvvogdq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bgkgbmaa.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2uhtqfoae.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2xuszqwro.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tvtpnqfy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2nwezbrnp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2bmuyvrdy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ggsgbnsy.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hmugvhqw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2mvwkxvay.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ctppjneq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2leskhuxp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vwbzjlrp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2axxqvlog.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2wugfskmq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qibkjmtb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2xglhupfa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2qcrrwegp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2vhkeyahu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2tysxqtax.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2aohvffib.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhcsnnyv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2doivcthv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2xrhmmdjm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2srodqwfw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lojbivai.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2clnwaysf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qkqckgij.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ragcxydq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jlylnffu.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ocgwwkjb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cjjnihot.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rsuwnoam.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fzsjhici.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bhdrogep.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2grxwmjdr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zpgkhhhi.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2irssliqq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2okltmxdj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2grrncvkl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2sswebrcr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gbhscxtu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2szeptslp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2gvgcdluz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2pbjewfty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jiyfwxyz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wuynyiwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yksdyuhi.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2latoiojp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2yubzwqwm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2solmyefa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2abkzbobe.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2bgujxyxi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2bqkmxutq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2snohinij.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2lblkvsdo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2sejwewmw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rtbwjmsi.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2eqcwvzng.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2vqcowjxg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2nclersbr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2lpeiqmmy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2oeofxwtj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2qorsjwoo.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2krqhmpgt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2uqlxbytc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2lhijcdjp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ymppcdft.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2acpasdhs.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2hccwibzb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2nkpukmmc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2utugjhgm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2euwtzrtl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2kemwaqnd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2tiksrtuf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qdhnjxuc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ifsbokcx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2lvhvidhu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2eelgdfyc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2grbmxibc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2wsbpcbmz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2uwmlcwfz.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2hdntwnvy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ikpqoydy.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2xlhjlgme.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2oofugsjk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2atudfjwt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2lqpfopgq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ojiqvnwd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ctqzcnaj.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ixetzwwt.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2kbvquiqv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2dbjyhmiw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2imypvvkx.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2jceqhoiq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2anpasdyq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ftazekms.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ttrurwya.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2cmvcvjpe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2kgkodfhv.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2vatoflzy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2neojuyjd.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ppcgxsbm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2dfsqhnbt.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2uraxlxvf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2dhwxoiry.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2sjtjvoso.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2tnqsrfxs.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2foqgjxwx.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2mdhxhgmz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2laciziyb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2mhnvhlwf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2sabpghsv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2rjdmthqa.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2qgczalfp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2oahehpnh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2nvqqgxuq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2hzkhbrxv.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2mmrmjiea.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2etnpgjvd.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2okpdnjwz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2mzozkymh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2rtfwqdlt.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2gpwumuvr.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2qjwakrgz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2vwcpidmg.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2mmhgpbjm.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2oqxjdemm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2rzsdhypv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2myjvkwaa.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2bsrrzdhj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2oexafprt.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nyrsdgmm.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2oqtfhrfi.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ucofgreq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2xlzydrfo.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2dunfffou.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2etlpshpg.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2khzwpeow.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2novyuqba.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2qobttzjj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2jxgqiyxg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2apvwvzsz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2dwjpqvmw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2cjaibuob.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2higyrmrq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2dknjmach.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrmmkbhl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2aqoavecu.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2wdnzvthb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zmpqidfu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2liwpwegy.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2hbwsnqty.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2oiucfdap.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2pvckcvaj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2kurwyexu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ojgjbqax.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2apljomqw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2bscngyuv.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jfwszwsn.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zjqucism.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2nttqtpmi.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2eronwydz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mvwadrab.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2kmurlitf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2cganlhjl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2yjqrtexk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2csrrqbme.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ytdfcgmh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lghgwmnv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2dbubfwmt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2jjmlmcji.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2neypxxkw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2elemyiup.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yzgrtbkn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2bgiwmgta.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2bpmvyobz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2smcqowrm.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2giwtfhvo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2twhpskoq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2tihuxkcg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2sjekzbcj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2fzzstdph.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2lntspijn.html


<!-- 参考信息 -->